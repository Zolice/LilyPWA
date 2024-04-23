<template>
  <div class="dropdown dropdown-hover">
    <div tabindex="0" role="button" class="btn m-1">{{ selected }}</div>
    <!-- <ul tabindex="0" class="flex flex-row h-32 overflow-auto dropdown-content z-[1] menu p-2 shadow bg-base-100 rounded-box w-64"> -->
    <ul tabindex="0"
      class="dropdown-content z-[1] flex flex-col p-2 shadow bg-base-100 rounded-box w-64 overflow-auto h-96 h-max-screen">
      <li v-for="item in models" :key="item" class="menu-title">
        <button class="active" @click="selectModel(item.id)">{{ item.id }}</button>
        <!-- v-if="item.id == selected"  -->
        <!-- <button v-else @click="selectModel(item.id)">{{ item.id }}</button> -->
      </li>
    </ul>


  </div>
</template>

<script setup lang="ts">

const models = ref([]);
const selected = ref("Loading...");
models.value = [{
  id: "Loading brain cells..."
}]

const apiKey = ref("")

// call the openapi using existing api key to find available models
// https://api.openai.com/v1/models \
//   -H "Authorization: Bearer $OPENAI_API_KEY"

onMounted(async () => {
  apiKey.value = localStorage.getItem("apiKey") ?? ""
  console.log(apiKey.value)
  const response = await fetch('https://api.openai.com/v1/models', {
    headers: {
      'Authorization': `Bearer ` + apiKey.value
    }
  });

  if (response.ok) {
    let data = await response.json();
    // models.value = await response.json();
    // console.log(models.value.data)
    console.log(data);
    // models.append(data.data);

    models.value = data.data;
    models.value = [...models.value].sort((a, b) => a.id.localeCompare(b.id));

    console.log(models)
    console.log("fetched")

    // Check for previous selectedmodel
    if (localStorage.getItem("selectedModel")) {
      // Check if the selectedmodel is available
      if (models.value.find((model: any) => model.id === localStorage.getItem("selectedModel"))) {
        selected.value = localStorage.getItem("selectedModel");
      }
    }
    else { 
      selected.value = models.value[0].id;
    }
  } else {
    console.error('Failed to fetch models', response.status, response.statusText);
    models.value = [{
      id: "Failed to fetch models!"
    },
    {
      id: "Check your API key."
    }
    ]
    selected.value = "Failed to fetch models!";
  }
});

const selectModel = (model: string) => {
  if (model === "Loading brain cells...") return;

  if (model === "Failed to fetch models!" || model === "Check your API key.") {
    return;
    // Open the settings page
  }

  selected.value = model;
  localStorage.setItem("selectedModel", model);
  console.log(selected.value)
}
</script>
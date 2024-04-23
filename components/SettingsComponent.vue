<template>
    <input type="checkbox" id="my_modal_7" class="modal-toggle" />
    <div class="modal" role="dialog">

        <div class="modal-box">
            <!-- <figure><img src="https://daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.jpg" alt="car!" />
            </figure> -->
            <!-- <div class="card-body"> -->
            <h2 class="card-title">Settings</h2>
            <p>OpenAI API Key</p>
            <label class="input input-bordered flex items-center gap-2 my-4">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor"
                    class="w-4 h-4 opacity-70">
                    <path fill-rule="evenodd"
                        d="M14 6a4 4 0 0 1-4.899 3.899l-1.955 1.955a.5.5 0 0 1-.353.146H5v1.5a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1-.5-.5v-2.293a.5.5 0 0 1 .146-.353l3.955-3.955A4 4 0 1 1 14 6Zm-4-2a.75.75 0 0 0 0 1.5.5.5 0 0 1 .5.5.75.75 0 0 0 1.5 0 2 2 0 0 0-2-2Z"
                        clip-rule="evenodd" />
                </svg>
                <input class="grow" v-model="apiKey" type="password" />
            </label>
            <div class="card-actions justify-end">
                <button class="btn btn-primary" @click="saveClose()">Save and Close</button>
            </div>
            <!-- </div> -->

            <!-- <h3 class="text-lg font-bold">Hello!</h3>
            <p class="py-4">This modal works with a hidden checkbox!</p> -->
        </div>
        <label class="modal-backdrop" for="my_modal_7">Close</label>
    </div>

    <!-- <div class="modal" role="dialog">
        <div class="card w-96 glass modal">
            <figure><img src="https://daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.jpg" alt="car!" />
            </figure>
            <div class="card-body">
                <h2 class="card-title">Life hack</h2>
                <p>How to park your car at your garage?</p>
                <div class="card-actions justify-end">
                    <button class="btn btn-primary">Learn now!</button>
                </div>
            </div>
        </div>
    </div> -->
</template>

<script setup lang="ts">
const apiKey = ref("")

onMounted(async () => {
    apiKey.value = localStorage.getItem("apiKey") ?? "";
})
// localStorage.getItem("apiKey") ?? "";

const saveClose = () => {
    // console.log(apiKey.value)
    localStorage.setItem("apiKey", apiKey.value);
    // console.log("Trysave?")
    // console.log(localStorage.getItem("apiKey"))
}

</script>
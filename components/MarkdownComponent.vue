<template>
    <div class="flex flex-row gap-1 my-4 px-4 w-full xl:w-4/5 mx-auto">
        <img :src="$attrs.icon" alt="profile" class="rounded-full w-10 h-10 mr-2">
        <div class="flex flex-col">
            <p class="text-lg font-bold">{{$attrs.name}}</p>
            <p class="">{{ $attrs.text }}</p>
        </div>
    </div>
</template>

<script setup lang="ts">
const text = useAttrs().text;

// Render markdown text
const markdown = ref('');
const renderMarkdown = () => {
    // markdown.value = marked(text);
}
</script>
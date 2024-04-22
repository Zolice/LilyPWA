<template>
    <div class="flex flex-row gap-1">
        <img :src="$attrs.icon" alt="profile" class="rounded-full w-10 h-10 mx-2">
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
<template>
    <div class="flex flex-row w-full h-screen">
        <div class="bg-[#111] lg:w-1/5 w-1/4 sm:w-72 h-full flex flex-col p-4 space-y-4">
            <div class="flex flex-row space-x-2 border-[#222] border-2 rounded-full p-2">
                <span class="material-symbols-outlined ">search</span>
                <p class="w-full my-auto">Search History</p>
                <span class="material-symbols-outlined ">close</span>
            </div>
            <div class="h-full overflow-y-auto">
                <ul class="space-y-2">
                    <li class="btn btn-ghost w-full hover:bg-[#FFC989]">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                    <li class="btn btn-ghost w-full">Home</li>
                </ul>
            </div>
            <div class="flex flex-col space-x-2 p-2 pt-0 justify-between items-left">
                <p class="py-2 px-4">Tokens: 999,999,999</p>
                <div class="flex flex-row spece-x-2 items-center">
                    <img src="/LilyGPT.png" alt="profile" class="rounded-full w-10 h-10 mx-2">
                    <p class="text-lg font-bold">LilyGPT</p>
                    <label for="my_modal_7" class="btn btn-ghost ml-auto">
                        <span class="material-symbols-outlined ">settings</span>
                    </label>
                    <SettingsComponent />
                </div>

            </div>
        </div>
        <div class="bg-[#1E1E1E] w-full h-screen flex flex-col">
            <HeaderComponent />
            <div class="overflow-y-auto h-full mx-auto">
                <MarkdownComponent name="User" icon="/LilyGPT.png" text="test" />
                <MarkdownComponent name="User" icon="/LilyGPT.png"
                    text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas at ex in leo auctor laoreet. Nulla tempor nibh quis dictum volutpat. Etiam a ullamcorper est. Nulla libero massa, dapibus vitae ultricies vulputate, egestas eget purus. Donec tempor fringilla blandit. Suspendisse a rhoncus enim, tincidunt tempor tortor. Pellentesque elementum mauris a ante pulvinar tincidunt eget id nisl. Nam ac risus et urna euismod aliquam a nec metus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent placerat ipsum risus, nec pharetra tellus tempor ornare. Interdum et malesuada fames ac ante ipsum primis in faucibus. Phasellus fermentum, nunc dapibus dapibus dictum, velit magna commodo diam, id sagittis velit elit a nisi. Pellentesque molestie vestibulum odio ut sodales. Integer aliquam non purus ut mollis. " />
                <MarkdownComponent name="User" icon="/LilyGPT.png"
                    text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas at ex in leo auctor laoreet. Nulla tempor nibh quis dictum volutpat. Etiam a ullamcorper est. Nulla libero massa, dapibus vitae ultricies vulputate, egestas eget purus. Donec tempor fringilla blandit. Suspendisse a rhoncus enim, tincidunt tempor tortor. Pellentesque elementum mauris a ante pulvinar tincidunt eget id nisl. Nam ac risus et urna euismod aliquam a nec metus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent placerat ipsum risus, nec pharetra tellus tempor ornare. Interdum et malesuada fames ac ante ipsum primis in faucibus. Phasellus fermentum, nunc dapibus dapibus dictum, velit magna commodo diam, id sagittis velit elit a nisi. Pellentesque molestie vestibulum odio ut sodales. Integer aliquam non purus ut mollis. " />
                <MarkdownComponent name="User" icon="/LilyGPT.png"
                    text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas at ex in leo auctor laoreet. Nulla tempor nibh quis dictum volutpat. Etiam a ullamcorper est. Nulla libero massa, dapibus vitae ultricies vulputate, egestas eget purus. Donec tempor fringilla blandit. Suspendisse a rhoncus enim, tincidunt tempor tortor. Pellentesque elementum mauris a ante pulvinar tincidunt eget id nisl. Nam ac risus et urna euismod aliquam a nec metus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent placerat ipsum risus, nec pharetra tellus tempor ornare. Interdum et malesuada fames ac ante ipsum primis in faucibus. Phasellus fermentum, nunc dapibus dapibus dictum, velit magna commodo diam, id sagittis velit elit a nisi. Pellentesque molestie vestibulum odio ut sodales. Integer aliquam non purus ut mollis. " />
                <MarkdownComponent name="User" icon="/LilyGPT.png"
                    text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas at ex in leo auctor laoreet. Nulla tempor nibh quis dictum volutpat. Etiam a ullamcorper est. Nulla libero massa, dapibus vitae ultricies vulputate, egestas eget purus. Donec tempor fringilla blandit. Suspendisse a rhoncus enim, tincidunt tempor tortor. Pellentesque elementum mauris a ante pulvinar tincidunt eget id nisl. Nam ac risus et urna euismod aliquam a nec metus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent placerat ipsum risus, nec pharetra tellus tempor ornare. Interdum et malesuada fames ac ante ipsum primis in faucibus. Phasellus fermentum, nunc dapibus dapibus dictum, velit magna commodo diam, id sagittis velit elit a nisi. Pellentesque molestie vestibulum odio ut sodales. Integer aliquam non purus ut mollis. " />
                <MarkdownComponent name="User" icon="/LilyGPT.png"
                    text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas at ex in leo auctor laoreet. Nulla tempor nibh quis dictum volutpat. Etiam a ullamcorper est. Nulla libero massa, dapibus vitae ultricies vulputate, egestas eget purus. Donec tempor fringilla blandit. Suspendisse a rhoncus enim, tincidunt tempor tortor. Pellentesque elementum mauris a ante pulvinar tincidunt eget id nisl. Nam ac risus et urna euismod aliquam a nec metus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent placerat ipsum risus, nec pharetra tellus tempor ornare. Interdum et malesuada fames ac ante ipsum primis in faucibus. Phasellus fermentum, nunc dapibus dapibus dictum, velit magna commodo diam, id sagittis velit elit a nisi. Pellentesque molestie vestibulum odio ut sodales. Integer aliquam non purus ut mollis. " />
                <MarkdownComponent name="User" icon="/LilyGPT.png"
                    text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas at ex in leo auctor laoreet. Nulla tempor nibh quis dictum volutpat. Etiam a ullamcorper est. Nulla libero massa, dapibus vitae ultricies vulputate, egestas eget purus. Donec tempor fringilla blandit. Suspendisse a rhoncus enim, tincidunt tempor tortor. Pellentesque elementum mauris a ante pulvinar tincidunt eget id nisl. Nam ac risus et urna euismod aliquam a nec metus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent placerat ipsum risus, nec pharetra tellus tempor ornare. Interdum et malesuada fames ac ante ipsum primis in faucibus. Phasellus fermentum, nunc dapibus dapibus dictum, velit magna commodo diam, id sagittis velit elit a nisi. Pellentesque molestie vestibulum odio ut sodales. Integer aliquam non purus ut mollis. " />
            </div>

            <div class="m-2 mx-auto flex flex-row items-center border-2 border-[#555] rounded-lg w-full xl:w-4/5">
                <textarea placeholder="Don't be shy, ask meow about anything!" class="w-full p-4 bg-transparent h-16"
                    v-model="query" />
                <div class="btn btn-ghost">
                    <span class="material-symbols-outlined">upload</span>
                </div>
                <div class="btn btn-ghost">
                    <span class="material-symbols-outlined text-[#FFC989]">send</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
const test = ref('u bad bad')
const query = ref('')

definePageMeta({
    title: 'LilyPWA',
});

useHead({
    title: 'LilyPWA',
});

const openSettings = () => {
    console.log('open settings')
}
</script>


<!-- <div class="m-4 mx-auto flex flex-row items-center border-2 border-[#555] rounded-lg w-full">
    <textarea placeholder="Don't be shy, ask meow about anything!"
        class="w-full p-4 bg-transparent h-16" v-model="query"/>
    <div class="btn btn-ghost">
        <span class="material-symbols-outlined">upload</span>
    </div>
    <div class="btn btn-ghost">
        <span class="material-symbols-outlined text-[#FFC989]">send</span>
    </div>
</div> -->
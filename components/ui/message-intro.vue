<template>
    <div class="gap-4 mx-auto p-5 m-5 py-1 text-gray-800">
        <div class="flex flex-row">
            <h3 class="text-lg font-medium leading-6 text-gray-300 flex grow">Hacking Modern Life GPT
            </h3>
            <div class="flex bg-indigo-700 rounded text-white text-center p-2 btn-logout" v-if="user">
                <UiLogout />
            </div>
        </div>
        <p class="mt-2 md:max-w-2xl lg:max-w-2xl xl:max-w-3xl  text-sm text-gray-500">
           ChatGPT clone, built with Nuxt3, GPT3 and Stable Diffusion. if you
            have any questions or comments, <a class="underline text-indigo-300" href="https://discord.gg/fyA9tCc7K4"
                target="_blank">contact me on Discord</a>. More info is available on "<a
                class="underline text-indigo-300" target="_blank"
                href="https://youtube.com/@hml?sub_confirmation=1">Hacking Modern Life</a>", my YouTube channel. Enjoy!
        </p>
    </div>
</template>

<script setup lang="ts">
const user = useSupabaseUser();
</script>

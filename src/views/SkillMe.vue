<template>
    <h2 class="text-3xl font-bold mb-6 flex items-center">
        <svg class="w-8 h-8 mr-3" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z"></path>
        </svg>
        Habilidades
    </h2>

    <div class="flex flex-wrap justify-center gap-4">
        <div class="p-4 rounded-lg icon-container icon-html transform hover:scale-105 transition-transform duration-300">
            <img :src="IconHTML" alt="HTML" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">HTML</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-css transform hover:scale-105 transition-transform duration-300">
            <img :src="IconCSS" alt="CSS3" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">CSS3</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-javascript transform hover:scale-105 transition-transform duration-300">
            <img :src="IconJS" alt="JavaScript" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">JavaScript</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-php transform hover:scale-105 transition-transform duration-300">
            <img :src="IconPHP" alt="PHP" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">PHP</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-csharp transform hover:scale-105 transition-transform duration-300">
            <img :src="IconCSharp" alt="C#" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">C#</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-laravel transform hover:scale-105 transition-transform duration-300">
            <img :src="IconLaravel" alt="Laravel" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">Laravel</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-vue transform hover:scale-105 transition-transform duration-300">
            <img :src="IconVue" alt="Vue JS" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">Vue JS</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-netCore transform hover:scale-105 transition-transform duration-300">
            <img :src="IconNetCore" alt="ASP .NET Core" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">ASP .NET Core</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-mysql transform hover:scale-105 transition-transform duration-300">
            <img :src="IconMySQL" alt="MySQL" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">MySQL</p>
        </div>
        <div class="p-4 rounded-lg icon-container icon-git transform hover:scale-105 transition-transform duration-300">
            <img :src="IconGit" alt="Git" class="w-12 h-12 mx-auto mb-2" />
            <p class="text-center">Git</p>
        </div>
    </div>

</template>

<script setup>
import IconHTML from '@/assets/svg/html5.svg'
import IconCSS from '@/assets/svg/css.svg'
import IconJS from '@/assets/svg/javascript.svg'
import IconPHP from '@/assets/svg/php.svg'
import IconCSharp from '@/assets/svg/csharp.svg'
import IconLaravel from '@/assets/svg/laravel.svg'
import IconVue from '@/assets/svg/vue.svg'
import IconNetCore from '@/assets/svg/netCore.svg'
import IconMySQL from '@/assets/svg/mysql.svg'
import IconGit from '@/assets/svg/git.svg'
</script>

<style scoped></style>
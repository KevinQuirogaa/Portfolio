<template>
    <main class="container mx-auto mt-10 px-4 mb-12">
            <div class="flex flex-col items-center mb-8">
                <div class="flex items-center">
                    <img :src="fotoCV" alt="Kevin Quiroga" class="rounded-full w-20 h-20 mr-4 border-4 border-blue-400">
                    <h1 class="text-5xl font-bold">Kevin Gomez Quiroga<span class="text-blue-400">.</span></h1>
                </div>
                <div class="text-center">
                    <h2 class="text-3xl text-gray-400 mb-2">Desarrollador de Software</h2>
                    <div class="flex items-center justify-center text-blue-400 mb-4">
                        <span class="bg-blue-600 text-white px-3 py-1 rounded-full text-sm light-animation">
                            Disponible para trabajar
                        </span>
                    </div>
                    <p class="text-lg mb-6">
                        Soy un desarrollador de software con experiencia en la creación de APIs RESTful, el manejo de los diferentes tipos de estados de un Endpoint y su estructura, además de tener conocimientos en el diseño de bases de datos relacionales. He trabajado con tecnologías como <span class="text-blue-400">Laravel</span>, <span class="text-blue-400">Symfony</span>, <span class="text-blue-400">PHP</span>, <span class="text-blue-400">ASP.NET Core Web Api</span>, <span class="text-blue-400">JavaScript</span>, <span class="text-blue-400">React JS</span> y <span class="text-blue-400">MySQL</span>.
                    </p>
                    <div class="flex space-x-6 justify-center">
                        <a href="mailto:kgomezquiroga1@gmail.com" class="flex items-center text-white icon-link">
                            <img :src="IconGmail" alt="Gmail" class="w-6 h-6 mr-2">
                            kgomezquiroga1@gmail.com
                        </a>
                        <a href="https://www.linkedin.com/in/kevin-gomez-quiroga-279316302/" target="_blank" class="flex items-center text-white icon-link">
                            <img :src="IconLinkedIn" alt="LinkedIn" class="w-6 h-6 mr-2">
                            LinkedIn
                        </a>
                        <a href="https://github.com/KevinKiroga?tab=repositories" target="_blank" class="flex items-center text-white icon-link">
                            <img :src="IconGitHub" alt="GitHub" class="w-6 h-6 mr-2">
                            GitHub
                        </a>
                        <a href="KevinQuirogaCV.pdf" target="_blank" class="flex items-center text-white icon-link">
                            <img :src="IconCV" alt="Hoja de Vida" class="w-6 h-6 mr-2">
                            CV
                        </a>
                    </div>
                </div>
            </div>
        </main>
</template>

<script setup>
import fotoCV from '@/assets/images/fotoCV.jpeg'
import IconGmail from '@/assets/svg/gmail.svg'
import IconLinkedIn from '@/assets/svg/linkedin.svg'
import IconGitHub from '@/assets/svg/github.svg'
import IconCV from '@/assets/svg/cv.svg'
</script>

<style scoped>
.icon-link {
    transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
}

.icon-link:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
}

.light-animation {
    position: relative;
    display: inline-block;
    animation: pulse 2s infinite;
}

@keyframes pulse {
    0% {
        box-shadow: 0 0 0 0 rgba(0, 0, 255, 0.7);
    }

    70% {
        box-shadow: 0 0 0 15px rgba(0, 0, 255, 0);
    }

    100% {
        box-shadow: 0 0 0 0 rgba(0, 0, 255, 0);
    }
}
</style>
<template>
    <main class="container mx-auto mt-10 px-4 mb-12">
        <div class="flex flex-col items-center mb-8">
            <div class="flex flex-col items-center mb-6">
                <div class="relative mb-3">
                    <img :src="fotoCV" alt="Kevin Quiroga"
                        class="rounded-full w-32 h-32 object-cover border-4 border-blue-400 shadow-lg hover:shadow-xl transition-shadow duration-300">
                    <div class="absolute -bottom-2 -right-2 bg-blue-400 rounded-full p-2 shadow-md">
                        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7">
                            </path>
                        </svg>
                    </div>
                </div>
                <h1 class="text-5xl font-bold text-center"><span class="text-blue-400">&lt;</span>Kevin Gomez
                    Quiroga<span class="text-blue-400">/&gt;</span></h1>
            </div>
            <div class="text-center">
                <h2 class="text-3xl text-gray-400 mb-3">Programador Fullstack Junior</h2>
                <div class="flex items-center justify-center text-blue-400 mb-4">
                    <span class="bg-blue-600 text-white px-3 py-1 rounded-full text-sm light-animation">
                        Disponible para trabajar
                    </span>
                </div>
                <p class="text-lg mb-6">
                    Desarrollador Fullstack con experiencia en el desarrollo de aplicaciones web y gestión de bases de
                    datos. Especializado en la creación de APIs RESTful con arquitecturas MVC y N-Capas, utilizando
                    tecnologías como Laravel, ASP.NET Core, Angular y SQL Server.

                    Experto en optimización de código, pruebas unitarias y metodologías ágiles. Comprometido con la
                    calidad del software y la mejora continua, destacando por su capacidad de análisis y resolución de
                    problemas.
                </p>
                <div class="flex space-x-6 justify-center">
                    <a href="mailto:kgomezquiroga2@gmail.com" class="flex items-center text-white icon-link">
                        <img :src="IconGmail" alt="Gmail" class="w-6 h-6 mr-2">
                        kgomezquiroga2@gmail.com
                    </a>
                    <a href="https://www.linkedin.com/in/kevin-quiroga-b81824357/" target="_blank"
                        class="flex items-center text-white icon-link">
                        <img :src="IconLinkedIn" alt="LinkedIn" class="w-6 h-6 mr-2">
                        Kevin Quiroga
                    </a>
                    <a href="https://github.com/KevinQuirogaa" target="_blank"
                        class="flex items-center text-white icon-link">
                        <img :src="IconGitHub" alt="GitHub" class="w-6 h-6 mr-2">
                        KevinQuirogaa
                    </a>
                    <a :href="pdfUrl" target="_blank" class="flex items-center text-white icon-link">
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
import pdfUrl from '@/assets/document/KevinQuirogaCV.pdf';

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
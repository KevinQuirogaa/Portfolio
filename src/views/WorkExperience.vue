<template>
    <h2 class="text-3xl font-bold mb-6 flex items-center justify-between">
        <span class="flex items-center">
            <svg class="w-8 h-8 mr-3" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
            </svg>
                Experiencia Laboral
        </span>
    </h2>
            
    <div class="bg-gray-800 rounded-lg p-6">
        <div class="flex items-start">
            <img :src="LogoExperience" class="w-12 h-12 bg-gray-600 rounded-md mr-4 flex-shrink-0 overflow-hidden">
            <div class="flex-grow">
                <div class="flex items-center justify-between">
                    <h3 class="text-xl font-semibold">Desarrollador web</h3>
                    <span class="text-gray-500">Julio 2022 - Enero 2023</span>
                </div>
                <p class="text-gray-400">Gobernación de Risaralda</p>
                <p class="text-gray-200 text-justify">
                    Durante mi tiempo como desarrollador web en la Gobernación de Risaralda, trabajé en el diseño y desarrollo de interfaces de usuario responsivas utilizando HTML5, CSS3 y JavaScript. Implementé nuevas funcionalidades según los requerimientos del cliente y administré la base de datos con MySQL XAMPP. Además, resolví problemas técnicos del sitio web y realicé revisiones de código para facilitar la comprensión de futuros desarrolladores. Utilicé la arquitectura cliente-servidor con PHP para la lógica del sitio web y gestioné los cambios de código con Git.
                </p>
                <!--button class="text-blue-400 hover:underline mt-2">... ver más</button-->
            </div>
        </div>
    </div>
</template>

<script setup>
import LogoExperience from '@/assets/images/logo-experience.jpg'
</script>

<style></style>
<template>
    <h2 class="text-3xl font-bold mb-6 flex items-center justify-between">
        <span class="flex items-center">
            <svg class="w-8 h-8 mr-3 icon-animate" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
            </svg>
                <span class="title-animate">Experiencia Laboral</span>
        </span>
    </h2>
            
    <div class="bg-gray-800 rounded-lg p-6 experience-card">
        <div class="flex items-start">
            <img :src="LogoExperience" class="w-12 h-12 bg-gray-600 rounded-md mr-4 flex-shrink-0 overflow-hidden logo-animate">
            <div class="flex-grow">
                <div class="flex items-center justify-between">
                    <h3 class="text-xl font-semibold title-hover">Desarrollador web</h3>
                    <span class="text-gray-500 date-animate">Julio 2022 - Enero 2023</span>
                </div>
                <p class="text-gray-400 company-hover">Gobernación de Risaralda</p>
                <p class="text-gray-200 text-justify description-animate">
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

<style scoped>
.experience-card {
    transition: all 0.3s ease;
    border: 1px solid transparent;
}

.experience-card:hover {
    border-color: rgba(59, 130, 246, 0.3);
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
}

.icon-animate {
    transition: transform 0.3s ease;
}

.icon-animate:hover {
    transform: scale(1.1);
    color: #3b82f6;
}

.title-animate {
    position: relative;
    display: inline-block;
}

.title-animate::after {
    content: '';
    position: absolute;
    width: 0;
    height: 2px;
    bottom: -2px;
    left: 0;
    background-color: #3b82f6;
    transition: width 0.3s ease;
}

.title-animate:hover::after {
    width: 100%;
}

.logo-animate {
    transition: all 0.3s ease;
}

.logo-animate:hover {
    transform: scale(1.1);
    box-shadow: 0 0 10px rgba(59, 130, 246, 0.5);
}

.title-hover {
    transition: color 0.3s ease;
}

.title-hover:hover {
    color: #3b82f6;
}

.company-hover {
    transition: all 0.3s ease;
}

.company-hover:hover {
    color: #3b82f6;
    transform: translateX(5px);
}

.date-animate {
    transition: all 0.3s ease;
    padding: 2px 8px;
    border-radius: 4px;
}

.date-animate:hover {
    background-color: rgba(59, 130, 246, 0.1);
    color: #3b82f6;
}

.description-animate {
    transition: all 0.3s ease;
}

.description-animate:hover {
    transform: translateY(-2px);
}
</style>
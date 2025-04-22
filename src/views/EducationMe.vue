<template>
    <h2 class="text-3xl font-bold mb-6 flex items-center">
        <svg class="w-8 h-8 mr-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M12 14l9-5-9-5-9 5zm0 7l-8-4.5v-2.47l8 4.5 8-4.5v2.47L12 21z"></path>
        </svg>
        Educación
    </h2>

    <div class="space-y-8">
        <!-- Sección Universidad -->
        <div class="flex group hover:scale-[1.01] transition-transform duration-300 cursor-pointer"
            @mouseover="hoverEffect" v-for="(edu, index) in educations" :key="index">
            <div class="flex flex-col items-center mr-4">
                <div class="w-3 h-3 bg-blue-500 rounded-full animate-pulse"
                    :class="{ 'animate-bounce': currentHover === index }"></div>
                <div class="w-1 h-full bg-gray-600 transition-colors duration-300 group-hover:bg-blue-400"></div>
            </div>
            <div class="pb-8 w-full">
                <div class="flex justify-between items-center flex-wrap">
                    <h3
                        class="text-xl font-semibold text-blue-500 transition-colors duration-300 group-hover:text-blue-300">
                        {{ edu.title }}
                    </h3>
                    <p
                        class="text-sm px-2 py-1 rounded-lg bg-gray-800/50 transition-all duration-300 group-hover:bg-blue-900/30">
                        {{ edu.period }}
                    </p>
                </div>
                <p class="text-lg mb-2">{{ edu.institution }}</p>
                <p class="text-gray-300 mb-4 text-justify">
                    {{ edu.description }}
                </p>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const currentHover = ref(null);

const hoverEffect = (index) => {
    currentHover.value = index;
    setTimeout(() => {
        currentHover.value = null;
    }, 1000);
};

const educations = [
    {
        title: 'Ingeniería de Sistemas',
        institution: 'Universidad Nacional Abierta y a Distancia - UNAD',
        period: 'Actualmente...',
        description: `  Como estudiante de Ingeniería de Sistemas en quinto semestre, he complementado mis
                        conocimientos previos adquiridos durante mi formación técnica y tecnológica con materias
                        como matemáticas, redes de datos, administración y organizaciones, entre otras. Al ser
                        homologado, no tuve que volver a cursar las materias que ya había aprobado en mi formación
                        previa. Todo esto me ha permitido continuar mi formación profesional de manera más completa
                        e integral, preparándome para enfrentar los desafíos del mundo laboral en el campo de la
                        Ingeniería de Sistemas.`
    },
    {
        title: 'Análisis y Desarrollo de Sistemas de Información',
        institution: 'SENA',
        period: 'Enero 2021 – Enero 2023 | Dosquebradas',
        description: `  Durante mi formación como Tecnólogo en ADSI, aprendí la lógica de programación, algoritmos,
                        diseño de bases de datos y análisis de requisitos, lo que me permitió desarrollar soluciones
                        efectivas para los clientes. También trabajé con diferentes lenguajes como PHP (Laravel),
                        Java (Java Web) y herramientas de desarrollo, lo que amplió mis habilidades y complementó
                        los conocimientos que obtuve durante mi formación técnica.`
    },
    {
        title: 'Técnico en Programación de Software',
        institution: 'SENA',
        period: 'Enero 2018 – Octubre 2020 | Pereira',
        description: ` Durante mi formación técnica, adquirí los conocimientos básicos de programación, incluyendo
                        la creación de páginas web con HTML5 y CSS3, el diseño de bases de datos con MySQL y Xampp,
                        y la creación de algoritmos con Pseint o diagramas de flujo. También aprendí los fundamentos
                        de PHP. Estas habilidades representaron mi primera experiencia en el mundo de la
                        programación y fueron unas bases para mi formación como Tecnólogo en ADSI.`
    }
];
</script>

<style scoped>
/* Animación suave al aparecer */
.v-enter-active {
    transition: opacity 0.5s ease, transform 0.5s ease;
}

.v-enter-from {
    opacity: 0;
    transform: translateY(20px);
}
</style>
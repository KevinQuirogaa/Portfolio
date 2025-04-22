<template>

    <h2 class="text-3xl font-bold mb-6 flex items-center">
        <svg class="w-8 h-8 mr-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"></path>
        </svg>
        Proyectos
    </h2>

    <div class="space-y-12 mb-10">
        <div class="flex items-center" v-for="(project, index) in projects" :key="index">
            <div class="w-1/2 pr-8">
                <img :src="project.image" :alt="project.title + ' Screenshot'"
                    class="project-image w-full h-60 object-cover rounded-lg shadow-lg" />
            </div>
            <div class="w-1/2 project-details">
                <h3 class="text-2xl font-bold mb-2">{{ project.title }}</h3>
                <div class="tags flex flex-wrap gap-2 mb-4">
                    <span v-for="(tag, tagIndex) in project.tags" :key="tagIndex"
                        class="px-2 py-1 bg-blue-800 text-white rounded-full text-sm">
                        {{ tag }}
                    </span>
                </div>
                <p class="text-gray-300 mb-6 text-justify">
                    {{ project.description }}
                </p>
                <div class="flex space-x-4 mb-4">
                    <a :href="project.githubUrl" target="_blank"
                        class="px-6 py-2 bg-gray-800 text-white rounded-md hover:bg-gray-700 transition duration-300 flex items-center justify-center">
                        <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 24 24"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 0C5.372 0 0 5.372 0 12c0 5.302 3.438 9.8 8.205 11.387.6.11.82-.26.82-.577v-2.174c-3.338.726-4.042-1.41-4.042-1.41-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.24 1.839 1.24 1.07 1.835 2.809 1.304 3.495.997.107-.775.418-1.305.762-1.605-2.665-.305-5.466-1.332-5.466-5.932 0-1.31.469-2.382 1.236-3.223-.124-.304-.535-1.527.117-3.176 0 0 1.008-.322 3.302 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.046.138 3.003.404 2.293-1.552 3.3-1.23 3.3-1.23.653 1.649.242 2.872.119 3.176.769.841 1.235 1.914 1.235 3.223 0 4.61-2.803 5.625-5.475 5.921.43.372.815 1.102.815 2.222v3.293c0 .32.22.693.825.574C20.565 21.795 24 17.298 24 12c0-6.628-5.373-12-12-12z">
                            </path>
                        </svg>
                        GitHub
                    </a>
                </div>
            </div>
        </div>
    </div>

</template>

<script setup>
import SenaProject from '@/assets/images/sena-project.png'
import BankingAPI from '@/assets/images/bankingAPI.jpg'
import DocumentAPI from '@/assets/images/documentAPI.jpg'
import PortfolioWEB from '@/assets/images/portfolioWEB.png'

const projects = [
    {
        title: 'Biometric - App',
        image: SenaProject,
        tags: ['Laravel', 'MySQL XAMPP', 'Bootstrap'],
        description: 'Un sistema educativo para gestionar estudiantes, instructores, fichas, asistencias mediante un código QR facilitando el seguimiento de los aprendices y la administración de la información académica.',
        githubUrl: 'https://github.com/KevinQuirogaa/BiometricApp'
    },
    {
        title: 'Banking API',
        image: BankingAPI,
        tags: ['ASP .NET CORE WEB API', 'SQL SERVER'],
        description: 'Es un sistema desarrollado para gestionar operaciones bancarias mediante una API RESTful. Permite administrar cuentas, clientes  y realizar transacciones , todo implementado con una arquitectura en capas.',
        githubUrl: 'https://github.com/KevinQuirogaa/BankingAPI'
    },
    {
        title: 'Document API',
        image: DocumentAPI,
        tags: ['Laravel', 'MySQL XAMPP', 'API RESTful'],
        description: 'Es un sistema desarrollado que permite gestionar documentos, ofrece funcionalidad de CRUD documentos, con un sistema de autenticación.',
        githubUrl: 'https://github.com/KevinQuirogaa/DocumentAPI'
    },
    {
        title: 'Portfolio WEB',
        image: PortfolioWEB,
        tags: ['Vue 3', 'Tailwind CSS', 'TypeScript'],
        description: 'Portafolio profesional desarrollado con Vue.js que presenta mi perfil como Desarrollador Fullstack Junior. Muestra mi experiencia, proyectos y habilidades con un diseño moderno e interactivo.',
        githubUrl: 'https://github.com/KevinQuirogaa/DocumentAPI'
    }
];
</script>

<style scoped>
.project-image {
    transition: transform 0.3s ease;
}

.project-image:hover {
    transform: scale(1.1);
}

.project-details {
    color: #ccc;
}

.project-details h3 {
    font-size: 1.5rem;
    font-weight: bold;
    margin-bottom: 0.5rem;
}
</style>
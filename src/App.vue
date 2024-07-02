<template>
   <div class="max-w-3xl mx-auto">
      <AboutMe />

      <div class="mb-12">
         <WorkExperience />
      </div>

      <div class="mb-12">
         <ProjectCode />
      </div>
      
      <div class="mb-12">
         <EducationMe />
      </div>

      <div class="mb-12">
         <SkillMe />
      </div>

   </div>
</template>

<script setup>
import AboutMe from './views/AboutMe.vue'
import WorkExperience from './views/WorkExperience.vue'
import EducationMe from './views/EducationMe.vue'
import ProjectCode from './views/ProjectCode.vue'
import SkillMe from './views/SkillMe.vue'
</script>

<style>

</style>

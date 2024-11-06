<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <div>
    <WelcomeItem>
      <template #icon>
        <DocumentationIcon />
      </template>
      <template #heading>Education</template>
      
      Attended Bowling Green State University to attain a degree from their
      <a href="https://www.bgsu.edu/academics/computer-science.html" target="_blank" rel="noopener">Computer Science bachelors</a>
      program. with a minor in General Science. 
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <ToolingIcon />
      </template>
      <template #heading>Job</template>

      Retained a job with  
      <a href="https://emprise1.com" target="_blank" rel="noopener">Emprise Technologies</a>
      in the fall of 2022 as a software Developer. Achieved Software Developer II position in the fall of 23.
      <br />

    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <EcosystemIcon />
      </template>
      <template #heading>Work</template>

      Currently training with 
      <a href="https://vuejs.org" target="_blank" rel="noopener">Vue </a>
      tools and tutorials to make best use of downtime between project assignments. 
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <CommunityIcon />
      </template>
      <template #heading>Hobbies</template>

      Participates in a variety of activities including team member of company employee 
      organized volleyball league in downtown Toledo at The Dock, and playing through 
      the beta game 
      <a href="https://palia.com/" target="_blank" rel="noopener">Palia</a>.
    </WelcomeItem>
  </div>
</template>

<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'

</script>

<template>
  <!-- cards -->
  <div class="mother-component">

    <WelcomeItem>
      <template #icon>
        <DocumentationIcon />
      </template>
      <template #heading>Custom analytics
      </template>
      Get a complete sales dashboard in the cloud. See activity, revenue and social metrics all in one place.
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <ToolingIcon />
      </template>
      <template #heading>Team Management
      </template>
      Our calendar lets you know what is happening with customer and projects so you are able to control process.
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <ToolingIcon />
      </template>
      <template #heading>Team Management
      </template>
      Our calendar lets you know what is happening with customer and projects so you are able to control process.
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <ToolingIcon />
      </template>
      <template #heading>Team Management
      </template>
      Our calendar lets you know what is happening with customer and projects so you are able to control process.
    </WelcomeItem>
  </div>
</template>

<style scoped lang="scss">
.mother-component {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 10px;
  margin-top: 4rem;


  @media (max-width: 1024px) {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>

<script setup>
import WelcomeItem from './WelcomeItem.vue'
import cardHeadingContent from './cardHeadingContent.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
</script>


<!-- cards heading content -->
<template class="card-container">

  <div class="card-heading-content">
    <cardHeadingContent>
      <template class="card-content-sub" #subheading>HOW IT WORKS</template>
    </cardHeadingContent>
    <cardHeadingContent>
      <template #heading>Gain more insight into how people use your</template>
    </cardHeadingContent>

  </div>
  <!-- cards -->
  <div class="card-component">

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
.card-container {
  margin-right: 2rem;
}

.card-component {

  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 10px;
  justify-content: end;


  @media (max-width: 1024px) {
    grid-template-columns: repeat(1, 1fr);
  }
}

.card-content-sub {
  color: var(--vt-c-white);
  background: var(--color-background-soft);
  border-radius: 10px;

}
</style>

<template>

  <div class="details">

    <h1>
      <slot name="heading"></slot>
    </h1>

    <h6>
      <slot name="subheading"></slot>
    </h6>


  </div>
</template>

<style scoped lang="scss">
.details {
  flex: 1
}

h1 {
  font-size: 3rem;
  font-weight: 900;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

h6 {
  font-size: 1rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}
</style>

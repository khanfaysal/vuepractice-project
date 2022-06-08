<template>
  <div class="worksCards">
    <div class="item">
      <i>
        <slot name="icon"></slot>
      </i>
      <div class="details">

        <h1>
          <slot name="subheading"></slot>
        </h1>

        <h3>
          <slot name="heading"></slot>
        </h3>

        <h6>
          <slot name="smallHeading"></slot>
        </h6>

        <slot></slot>
      </div>
    </div>
  </div>
</template>

<style scoped>
.worksCards {
  width: 100%;
}

.item {
  margin-top: 2rem;
}

.details {
  flex: 1
}

i {
  display: flex;
  place-items: center;
  place-content: center;
  width: 32px;
  height: 32px;
  color: var(--color-text);
}

h1 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

h3 {
  font-size: 1.2rem;
  font-weight: 900;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

h6 {
  font-size: 5rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

@media (min-width: 1024px) {

  i {
    color: var(--vt-c-white);
    background: var(--color-background-soft);
    border-radius: 50%;
    width: 50px;
    height: 50px;
  }


}
</style>

<template>
  <div class="intro">
    <div class="intro__illustration"></div>
    <div class="intro__title">
      <h1>All your files in one secure location, accessible anywhere.</h1>
    </div>
    <div class="intro__description">
      <p class="description">Fylo stores all your most important files in one secure location. Access them whereever you need, share and collaborate with friends family, and co-workers.</p>
      <button class="btn-default">Get Started</button>
    </div>
  </div> 
</template>

<script>
export default {

}
</script>

<style lang="scss">
.intro {
  padding: 20px 30px;
  display: grid;
  justify-items: center;
  background-image: url('../images/bg-curvy-mobile.svg');
  background-size: contain;
  background-repeat: no-repeat;
  background-position: bottom;
  background-color: var(--dark-blue);

  &__title {
    font-size: 0.75rem;
    letter-spacing: 0.4px;
    max-width: 500px;
  }

  &__illustration {
    background-image: url('../images/illustration-intro.png');
    background-size: contain;
    background-repeat: no-repeat;
    width: 100%;
    height: 250px;
    max-width: 500px;
  }

  &__description {
    letter-spacing: 0.5px;
    max-width: 500px;
  }
}
</style>
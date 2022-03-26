<template>
  <div class="testimonials">
    <div class="testimonials__productive"></div>
    <div class="testimonials__content">
      <h2 class="testimonials__content__title">Stay productive, whereever you are</h2>
      <p class="testimonials__content__description">Never let location be an issue when accessing your files. Fylo has you covered for all of your file storage needs.</p>
      <p class="testimonials__content__description--second">Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.</p>
      <a href="#" class="testimonials__content__works">See how Fylo works</a>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.testimonials {
  padding: 0 30px;
  margin-bottom: 120px;
  display: grid;
  justify-items: center;

  &__productive {
    width: 320px;
    height: 250px;
    background-image: url('../images/illustration-stay-productive.png');
    background-repeat: no-repeat;
    background-size: contain;
  }

  &__content {
    text-align: left;
    max-width: 500px;

    &__title {
      font-size: 1.29rem;
      max-width: 250px;
    }

    &__works {
      width: 160px;
      display: grid;
      grid-template-columns: repeat(2, auto);
      grid-template-rows: auto;
      column-gap: 10px;
      align-items: center;
      text-decoration: none;
      color: hsl(176, 68%, 64%);
      border-bottom: 1px solid hsl(176, 68%, 64%);

      &:after {
        content: '';
        width: 16px;
        height: 16px;
        background-image: url('../images/icon-arrow.svg');
      }
    }
  }
}
</style>
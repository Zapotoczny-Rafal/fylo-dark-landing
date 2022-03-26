<template>
  <div class="container">
    <div class="modal">
      <h2 class="modal__title">Get early access today</h2>
      <div class="modal__description">It only takes a minute to sign up and our free starter tier is extremely generous. If you have any questions, our support team would be happy to help you.</div>
      <form action="#" method="post">
        <input type="text" class="modal__input" placeholder="email@example.pl">
        <button class="btn-default btn-modal">Get Started for free</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.container {
  display: flex;
  justify-content: center;

  .modal {
    width: 320px;
    height: 330px;
    border-radius: 12px;
    padding: 15px;
    background-color: var(--dark-blue-test);
    display: grid;
    justify-items: center;
    grid-template-columns: auto;
    grid-template-rows: repeat(3, auto);
    position: relative;
    top: 180px;
    z-index: 1000;

    &__title {
      font-size: 1.375rem;
    }

    &__description {
      margin-bottom: 20px;
    }

    &__input {
      margin-bottom: 10px;
    }

    input {
      width: 288px;
      height: 45px;
      font-family: 'Open Sans', sans-serif;
      border: none;
      border-radius: 45px;
      padding-left: 20px;
      grid-area: input;

      &::-moz-placeholder {
        font-size: 12px;
      }

      &::-webkit-input-placeholder {
        font-size: 12px;
      }
    }

    .btn-modal {
      width: 310px;
    }
  }
}
</style>
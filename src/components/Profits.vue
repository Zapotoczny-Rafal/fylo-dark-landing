<template>
  <div class="profits">
    <div class="profit">
      <div class="profit__icon profit__icon--access"></div>
      <h2 class="profit__title">Access your files, anywhere</h2>
      <p class="profit__description">The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.</p>
    </div>
    <div class="profit">
      <div class="profit__icon profit__icon--security"></div>
      <h2 class="profit__title">Security you can trust</h2>
      <p class="profit__description">2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.</p>
    </div>
    <div class="profit">
      <div class="profit__icon profit__icon--time"></div>
      <h2 class="profit__title">Real-time collaboration</h2>
      <p class="profit__description">Securely share files and folders with frinds, family and colleagues for live collaboration. No email attachments required.</p>
    </div>
    <div class="profit">
      <div class="profit__icon profit__icon--story"></div>
      <h2 class="profit__title">Story any type of file</h2>
      <p class="profit__description">Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.profits {
  display: grid;
  justify-items: center;
  padding: 0px 30px;
  margin-bottom: 70px;
  padding-top: 80px;

  .profit {
    margin-bottom: 50px;
    display: grid;
    justify-items: center;
    max-width: 400px;

    &__title {
      font-size: 1.375rem;
    }

    &__icon {
      background-repeat: no-repeat;
      width: 85px;
      height: 88px;

      &--access {
        background-image: url('../images/icon-access-anywhere.svg');
      }

      &--security {
        background-image: url('../images/icon-security.svg');
      }

      &--time {
        background-image: url('../images/icon-collaboration.svg');
      }

      &--story {
        background-image: url('../images/icon-any-file.svg');
      }
    }
  }
}
</style>
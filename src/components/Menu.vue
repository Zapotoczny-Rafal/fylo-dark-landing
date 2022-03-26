<template>
  <div class="menu">
    <div class="menu__logo" href="#"></div>
    <div class="menu__items">
      <a class="item" href="#">Features</a>
      <a class="item" href="#">Team</a>
      <a class="item" href="#">Sign In</a>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.menu {
  height: 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  background-color: var(--dark-blue);

  &__logo {
    width: 88px;
    height: 26px;
    background-image: url('../images/logo.svg');
    background-size: 88px 26px;
    cursor: pointer;
  }

  &__items {
    display: flex;
    align-items: center;

    a {
      font-size: 12px;
    }

    a + a {
      margin-left: 25px;
    }
  }
}
</style>
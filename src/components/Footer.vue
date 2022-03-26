<template>
  <footer class="footer">
    <div class="footer__logo"></div>
    <div class="footer__main">
      <div class="footer__content">
        <div class="footer__content__item">
          <p class="icon icon-location"></p>
          <p class="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
        </div>
        <div class="second">
          <div class="footer__content__item">
            <p class="icon icon-phone"></p>
            <p class="text">+1-543-123-4567</p>
          </div>
          <div class="footer__content__item">
            <p class="icon icon-email"></p>
            <p class="text">example@fylo.com</p>
          </div>
        </div> 
      </div>
      <nav class="footer__vertical-menu">
        <div class="first">
          <div class="item">
            <a href="#">About Us</a>
            </div>
          <div class="item">
            <a href="#">Jobs</a>
            </div>
          <div class="item">
            <a href="#">Press</a>
            </div>
          <div class="item">
            <a href="#">Blog</a>
          </div>
        </div>
        <div class="second">
          <div class="item">
            <a href="#">Contact Us</a>
            </div>
          <div class="item">  
            <a href="#">Terms</a>
            </div>
          <div class="item">
            <a href="#">Privacy</a>
          </div>
        </div>  
      </nav>
      <div class="footer__social">
        <div class="footer__social__icon">
          <ion-icon name="logo-facebook"></ion-icon>
        </div>
        <div class="footer__social__icon">
          <ion-icon name="logo-twitter"></ion-icon>
        </div>
        <div class="footer__social__icon">
          <ion-icon name="logo-instagram"></ion-icon>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.footer {
  background-color: var(--dark-blue-footer);
  display: grid;
  grid-template-columns: auto;
  grid-template-rows: repeat(2, auto);
  grid-template-areas: "footer__logo" "footer__main";
  row-gap: 10px;
  position: relative;
  bottom: -14px;
  padding: 0 30px;

  &__main {
    display: grid;
  }

  &__content {
    display: grid;
    grid-template-columns: auto;
    grid-template-rows: repeat(3, auto);
    justify-items: start;
    margin-bottom: 80px;

    .icon {
      width: 20px;
      height: 20px;
      background-repeat: no-repeat;
      background-position: center;
    }

    &__item {
      display: grid;
      grid-template-columns: 38px 280px;
      grid-template-areas: "icon text";
    }

    .icon-location {
      background-image: url('../images/icon-location.svg');
    }

    .icon-phone {
      background-image: url('../images/icon-phone.svg');
    }
    .icon-email {
      background-image: url('../images/icon-email.svg');
    }

    p {
      font-size: 1.125rem;
      text-align: left;
    }
  }

  &__logo {
    background-image: url('../images/logo.svg');
    background-repeat: no-repeat;
    background-position: 10px 240px;
    width: 300px;
    height: 110px;
    padding-bottom: 200px;
  }

  &__vertical-menu {
    display: grid;
    justify-items: start;
    margin-bottom: 30px;

    .first, .second {
      display: grid;
      justify-items: start;
      max-height: 120px;
    }

    .first {
      margin-bottom: 50px;
    }

    .item {
      margin-bottom: 12px;
      height: 28px;

      a {
        font-size: 1.175rem;
      }

    }
  }

  &__social {
    display: flex;
    height: 120px;
    align-items: center;
    justify-content: center;

    &__icon {
      font-size: 16px;
      width: 30px;
      height: 30px;
      border-radius: 50%;
      border: 1px solid var(--white);
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
    }

    div + div {
      margin-left: 10px;
    }
  }
}
</style>
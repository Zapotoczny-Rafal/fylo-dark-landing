<template>
  <Menu />
  <Intro />
  <Profits />
  <Testimonials />
  <Comments />
  <Modal />
  <Footer />
</template>

<script>
import Intro from './components/Intro.vue';
import Menu from "./components/Menu.vue";
import Profits from './components/Profits.vue';
import Testimonials from './components/Testimonials.vue';
import Comments from './components/Comments.vue';
import Modal from './components/Modal.vue';
import Footer from './components/Footer.vue';


export default {

  name: 'App',
  components: {
    Menu,
    Intro,
    Profits,
    Testimonials,
    Comments,
    Modal,
    Footer
}
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&family=Raleway:wght@400;700&display=swap');

:root {
  --dark-blue: hsl(217, 28%, 15%);
  --dark-blue-main: hsl(218, 28%, 13%);
  --dark-blue-footer: hsl(216, 53%, 9%);
  --dark-blue-test: hsl(219, 30%, 18%);

  --cyan: hsl(176, 68%, 64%);
  --blue: hsl(198, 60%, 50%);
  --light-red: hsl(0, 100%, 63%);
  --white: hsl(0, 0%, 100%);
} 

body,html {
  font-size: 14px;
}

body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: 'Open Sans', sans-serif;
  background-color: var(--dark-blue-main);
  color: var(--white);
}

button {
  border: none;
  cursor: pointer;
}

a {
  color: var(--white);
  text-decoration: none;
}

.btn-default {
  width: 250px;
  height: 50px;
  border-radius: 25px;
  color: var(--white);
  background: linear-gradient(90deg, var(--cyan), var(--blue));
  font-weight: 700;
  margin-top: 1rem;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

@media screen and (min-width: 376px) {
.intro {
  background-image: url('images/bg-curvy-desktop.svg');

  &__illustration {
    height: 300px;
  }
}
}

@media screen and (min-width: 751px) {
.intro {
  &__illustration {
    height: 500px;
  }

  &__title, &__description {
    position: relative;
    bottom: 100px;
  }
}

.profits {
  grid-template-columns: repeat(2, auto);
  padding: 0px 20%;
}

.testimonials {
  grid-template-columns: repeat(2, auto);
  padding: 0px 12%;
  margin-bottom: 20px;

  &__productive {
    width: 500px;
    height: 500px;
  }

  &__content__title {
    font-size: 1.5rem;
  }
}

.quote {
  left: -25%;
}

.comments {
  grid-template-columns: repeat(2, auto);
  padding: 0px 16%;
  gap: 10px;
}

}

@media screen and (min-width: 1440px) {
.comments {
    grid-template-columns: repeat(3, auto);
}

.container .modal {
  width: 60%;
  height: 240px;

  &__title {
    font-size: 1.625rem;
  }

  &__description {
    width: 675px;
  }

  .btn-modal {
    width: 200px;
  }

  input {
    position: relative;
    right: 30px;
    width: 520px;
  }
}

.footer {
  padding: 0px 70px 0px 150px;

  &__content {
    grid-template-columns: 380px 320px;
    column-gap: 70px;

    &__item {
      grid-template-columns: 38px 320px;
    }
  }

  &__main {
    grid-template-columns: 740px 260px 180px;
    grid-template-rows: auto;
    grid-template-areas: "footer__content footer__vertical-menu footer__social";
    column-gap: 10px;
    height: 270px;
  }

  &__vertical-menu {
    grid-template-columns: repeat(2, auto);
    column-gap: 40px;
  }
}
}
</style>

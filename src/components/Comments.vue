<template>
  <div class="quote"></div>
  <div class="comments">
    <div class="comment">
      <div class="comment__content">Fylo has improved our team productivy by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.</div>
      <div class="comment__author">
        <div class="comment__author__image comment__author__image--satish img"></div>
        <div class="info">
          <p class="name">Satish Patel</p>
          <span class="company">Founder & CEO, Huddle</span>
        </div>
      </div>
    </div>
    <div class="comment">
      <div class="comment__content">Fylo has improved our team productivy by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.</div>
      <div class="comment__author">
        <div class="comment__author__image comment__author__image--bruce img"></div>
        <div class="info">
          <p class="name">Bruce McKenzie</p>
          <span class="company">Founder & CEO, Huddle</span>
        </div>
      </div>
    </div>
    <div class="comment">
      <div class="comment__content">Fylo has improved our team productivy by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.</div>
      <div class="comment__author">
        <div class="comment__author__image comment__author__image--iva img"></div>
        <div class="info">
          <p class="name">Iva Boyd</p>
          <span class="company">Founder & CEO, Huddle</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.quote {
    height: 23px;
    background-image: url('../images/bg-quotes.png');
    background-repeat: no-repeat;
    background-position: center center;
    background-size: 27px 22px;
    position: relative;
    left: -135px;
}

.comments {
  padding: 0 20px;
  display: grid;
  justify-items: center;

  .comment {
    width: 280px;
    height: 150px;
    padding: 20px;
    background-color: var(--dark-blue-test);
    border-radius: 8px;
    margin-bottom: 30px;

    &__content {
      text-align: left;
      font-size: 0.875rem;
      margin-bottom: 20px;
    }

    &__author {
      display: grid;
      grid-template-columns: 50px 180px;
      grid-template-rows: 50px;
      grid-template-areas: "img info";
      align-items: center;
      text-align: left;

      &__image {
        width: 36px;
        height: 36px;
        background-position: center;
        background-size: 36px 36px;
        border-radius: 50%;

        &--satish {
          background-image: url('../images/profile-1.jpg');
        }

        &--bruce {
          background-image: url('../images/profile-2.jpg');
        }

        &--iva {
          background-image: url('../images/profile-3.jpg');
        }
      }

      .name {
        font-weight: 700;
        letter-spacing: 0.8px;
        margin:0px;
      }

      .company {
        font-size: 13px;
        font-weight: 400;
        letter-spacing: 0.5px;
      }
    }
  }
}
</style>
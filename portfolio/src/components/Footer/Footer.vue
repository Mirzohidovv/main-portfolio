<template>
  <footer class="footer">
    <div class="container">
      <ul class="footer__list">
        <a
          href="https://www.facebook.com/"
          class="footer__links"
          target="_blank"
          >Facebook</a
        >
        <a
          href="https://www.instagram.com/mirzohidov_r/"
          class="footer__links"
          target="_blank"
          >Instagram</a
        >
        <a
          href="https://www.youtube.com/@mirzohidov_r4456"
          class="footer__links"
          target="_blank"
          >Youtube</a
        >
      </ul>
    </div>
  </footer>
</template>

<script setup></script>

<style lang="scss" scoped>
.footer {
  background: #333;

  &__list {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    column-gap: 18px;
  }
  &__links {
    padding-top: 15px;
    padding-bottom: 23px;
    color: rgba(255, 255, 255, 0.5);
    font-family: Poppins;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 35px;
    cursor: pointer;
    transition: 0.3s all;
    &:hover {
      color: #fff;
    }
  }
}
</style>

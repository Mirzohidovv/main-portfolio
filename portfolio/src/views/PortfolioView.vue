<template>
  <section class="portfolio">
    <h1 class="title">Portfolio</h1>

    <div class="portfolio__content container">
      <h2 class="portfolio__content-title">Gallery</h2>
      <div class="portfolio__content-line"></div>

      <ul>
        <li class="portfolio__content-list">
          <a href="">All</a>
          <a href="">Web-Applications</a>
          <a href="">Web-Sites</a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script setup>
import { ref, reactive } from "vue";

const Links = reactive([
  { id: 1, title: "All", path: "/portfolio/all" },
  { id: 2, title: "Web-Applications", path: "/portfolio/web-aplications" },
  { id: 3, title: "Web-Sites", path: "/portfolio/web-sites" },
]);
</script>

<style lang="scss" scoped>
.title {
  color: #fff;
  font-family: Poppins;
  font-size: 55px;
  font-style: normal;
  font-weight: 700;
  line-height: 35px;
  padding: 92px 0;
  padding-left: 62px;
  background: #252525;
  border-bottom: 1px solid #343333;
}
.portfolio {
  margin: 100px 0;

  &__content {
    display: flex;
    flex-direction: column;
    margin-left: 100px;
    row-gap: 30px;
    margin-top: 80px;

    &-title {
      color: #fff;
      font-family: Poppins;
      font-size: 28px;
      font-style: normal;
      font-weight: 700;
      line-height: 35px;
      max-width: 150px;
      position: relative;
      
      &::after {
        content: "";
        background: #007ced;
        width: 30%;
        border-radius: 4px;
        display: block;
      }
    }
    
    &-line::after {
      content: "";
      position: absolute;
      height: 100%;
      top: 0;
      left: 0;
      border-radius: 8px;
    }

    &-list {
      display: flex;
      column-gap: 30px;
    }
  }
}
</style>

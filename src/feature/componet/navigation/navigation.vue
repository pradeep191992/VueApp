<template>
  <nav class="header">
    <!-- {{NUMBER_ONE}}
    <button @click="name">Click Me</button>-->
    <ul class="nav-list">
      <li class="nav-list-item">
        <a href="/">Discover</a>
      </li>
      <li class="nav-list-item">
        <a href="/">Room Ideas</a>
        <ul>
          <li>
            <a href="/">Room Ideas 1</a>
          </li>
          <li>
            <a href="/">Room Ideas 2</a>
          </li>
          <li>
            <a href="/">Room Ideas 3</a>
          </li>
          <li>
            <a href="/">Room Ideas 4</a>
          </li>
          <li>
            <a href="/">Room Ideas 5</a>
          </li>
        </ul>
      </li>
      <li class="nav-list-item">
        <a href="/">Trends</a>
        <ul>
          <li>
            <a href="/"></a>
          </li>
        </ul>
      </li>
      <li class="nav-list-item">
        <a href="/">Icon</a>
      </li>
      <li class="nav-list-item">
        <a href="/">Icon 2</a>
      </li>
      <li class="nav-list-item">
        <a href="/">...</a>
        <ul>
          <li>
            <a href="/">Blog</a>
          </li>
          <li>
            <a href="/">See Terms and Privacy</a>
          </li>
        </ul>
      </li>
    </ul>
  </nav>
</template>

<script>
import headerconstant from "./../../constant/navigation.constant.ts";
export default {
  name: "Navigation",
  // components: {
  //   Navigation
  // }
  data() {
    return {
      NUMBER_ONE: "HOme"
    };
  },
  methods: {
    name() {
      console.log(headerconstant);
    }
  },
  created() {
    // this.NUMBER_ONE = headerconstant;
    console.log(headerconstant);
  }
};
</script>

<style lang="scss" scoped>
.nav-list {
  display: flex;
  align-items: center;
  &-item {
    position: relative;
    a {
      font-size: 16px;
      padding: 10px 20px;
      text-decoration: none;
    }
    ul {
      display: none;
      background-color: #fff;
      position: absolute;
      right: 0;
      padding: 8px 0;
      border: 1px solid #e0e0e0;
      min-width: 220px;
      z-index: 13;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
    }
    &:hover {
      ul {
        display: block;
      }
    }
  }
}
</style>
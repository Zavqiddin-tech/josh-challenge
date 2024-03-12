<template>
  <div class="nav">
    <div class="nav-hero flex wrap items-center justify-between">
      <div class="logo flex items-center">
        <img src="@/assets/image/nav-logo.svg" alt="" />
        <div class="logo-title">Marico</div>
      </div>
      <ul class="nav-ul">
        <li>
          <a class="nav-ul-down flex items-center" href="#"
            >Use Cases <i class="bx bxs-chevron-down"></i
          ></a>
        </li>
        <li><a href="#">About</a></li>
        <li><a href="#">Pricing</a></li>
        <li><a href="#">Blog</a></li>
      </ul>
      <div class="nav-btns">
        <button class="btn small-gray">Login</button>
        <button class="btn small">Sign Up</button>
      </div>
      <div class="hamburger" @click="openMenu()">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
      </div>
    </div>
    <div class="hamburger-menu">
      <ul :class="`${toggle ? 'hamburger-ul active' : 'hamburger-ul'}`">
        <li>
          <a class="nav-ul-down flex items-center" href="#"
            >Use Cases <i class="bx bxs-chevron-down"></i
          ></a>
        </li>
        <li><a href="#">About</a></li>
        <li><a href="#">Pricing</a></li>
        <li><a href="#">Blog</a></li>
        <div class="hamburger-btns">
          <button class="btn small-gray">Login</button>
          <button class="btn small">Sign Up</button>
        </div>
      </ul>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const toggle = ref(false);
const openMenu = () => {
  toggle.value = !toggle.value;
};
</script>

<style lang="scss">
@import "@/assets/styles/color.scss";
.nav {
  padding: 0 140px;
  &-ul {
    gap: 38px;
    display: flex;
    align-items: center;
    &-down {
      gap: 8px;
    }
    a {
      color: $gray;
      transition: 0.25s;
      font-size: 20px;
      &:hover {
        color: $blue-step;
      }
    }
  }
  .logo {
    gap: 17px;
  }
  .logo-title {
    font-size: 37px;
    font-weight: 800;
  }
}
.hamburger {
  width: 35px;
  height: 30px;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 6px;
  display: none;
  z-index: 2;

  .line {
    width: 100%;
    height: 3px;
    border-radius: 20px;
    background-color: #fff;
  }
}

.hamburger-ul {
  position: absolute;
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 10px;
  backdrop-filter: blur(15px);
  transform: translateY(-1000px);
  top: 0px;
  left: 0;
  transition: 0.3s;
  background-color: rgba(0, 0, 0, 0.5);
  &.active {
    transform: translateY(0px);
  }
  li {
    a {
      color: $gray;
      transition: 0.25s;
      font-size: 20px;
      &:hover {
        color: $blue-step;
      }
    }
  }
}

@media (max-width: 1100px) {
  .nav-btns {
    width: 100%;
    display: flex;
    justify-content: center;
    padding-top: 20px;
  }
}
@media (max-width: 1100px) {
  .nav {
    padding: 0 60px;
  }
}
@media (max-width: 750px) {
  .hamburger {
    display: flex;
  }
  .nav {
    padding: 0 60px;
    &-ul {
      display: none;
    }
    &-btns {
      display: none;
    }
  }
}
</style>

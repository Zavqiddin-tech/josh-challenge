<template>
  <div class="footer flex justify-between items-center">
    <div class="footer-left col-lg-12">
      <div class="footer-logo flex items-center">
        <img src="@/assets/image/footer-logo.png" alt="" />
        <div class="footer-logo-title">Marico</div>
      </div>
      <div class="footer-email">info@marico.co</div>
    </div>
    <ul class="footer-ul flex items-center col-lg-12">
      <li><a href="#">About</a></li>
      <li><a href="#">Pricing</a></li>
      <li><a href="#">Blog</a></li>
    </ul>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
@import "@/assets/styles/color.scss";
.footer {
    padding: 183px 140px 96px;
  &-logo {
    gap: 24px;
    &-title {
      font-size: 42px;
      font-weight: 800;
    }
  }
  &-email {
    padding-top: 14px;
    font-size: 27px;
    color: $gray;
  }
  &-ul {
    gap: 38px;
    &-down {
      gap: 8px;
    }
    a {
      color: $gray;
      transition: 0.25s;
      font-weight: 500;
      font-size: 28px;
      &:hover {
        color: $blue-step;
        
      }
    }
  }
}

@media (max-width: 750px) {
  .footer {
    flex-direction: column;
  &-logo {
    justify-content: center;
    gap: 24px;
    &-title {
      font-size: 35px;
      font-weight: 800;
    }
  }
  &-email {
    display: flex;
    justify-content: center;
    padding-top: 14px;
    font-size: 20px;
    color: $gray;
  }
  &-ul {
    gap: 38px;
    justify-content: center;
    &-down {
      gap: 8px;
    }
    a {
      color: $gray;
      transition: 0.25s;
      font-weight: 500;
      font-size: 18px;
      &:hover {
        color: $blue-step;
        
      }
    }
  }
}
}
</style>

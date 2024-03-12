<template>
  <div class="setup flex justify-center items-center column">
    <img src="@/assets/image/big-logo.svg" alt="" />
    <div class="setup-title text-center">Get Started Now</div>
    <div class="setup-subtitle text-center">Setup is easy and takes under 5 minutes.</div>
    <button class="btn big-blue">Get Started Now</button>
    <div class="setup-bottom flex items-center">
      <img src="@/assets/image/big-circle.png" alt="" />
      <div class="setup-number">1000+</div>
      <div class="setup-text">creators have already started</div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
@import "@/assets/styles/color.scss";
.setup {
    &-title {
        padding-top: 20px;
        font-size: 100px;
        font-weight: 700;
    }
    &-subtitle {
        padding-bottom: 15px;
        font-size: 43px;
    }
    .big-blue {
        padding: 28px 112px;
    }
    &-bottom {
        padding-top: 26px;
        gap: 11px;
    }
    &-number {
        font-size: 38px;
        font-weight: 700;
    }
    &-text {
        font-size: 38px;
        color: $gray;
    }
}

@media (max-width: 750px) {
  .setup {
    &-title {
      font-size: 50px;
    }
    &-subtitle {
        font-size: 30px;
    }
    &-number {
        font-size: 20px;
    }
    &-text {
        font-size: 20px;
    }
  }
}
</style>

<template>
  <div class="mobile">
    <div class="mobile-content flex">
      <div class="col-6">
        <div class="mobile-box">
          <div class="mobile-link">One Link</div>
          <div class="mobile-title">ALL You Create. <span>One Link</span></div>
          <img src="@/assets/image/mobile.png" alt="mobile" />
        </div>
      </div>
      <div class="col-6">
        <div class="mobile-box">
          <div class="mobile-link">Collect Subscribers</div>
          <div class="mobile-title bold">
            Emails. <br />
            Phone #s. <br />
            <span>All Yours.</span>
          </div>
        </div>
      </div>
    </div>
    <div class="mobile-btns flex justify-center">
      <button class="btn big-blue">Get Started</button>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss">
@import "@/assets/styles/color.scss";
.mobile {
  padding-top: 176px;
  padding-left: 94px;
  padding-right: 94px;
  padding-bottom: 189px;
  &-content {
    gap: 23px;
  }
  &-box {
    min-height: 666px;
    padding-top: 33px;
    padding-left: 45px;
    position: relative;
    background-color: #0d0d0d;
    img {
      width: 90%;
      position: absolute;
      right: 0px;
      bottom: 0px;
      object-fit: cover;
    }
  }
  &-link {
    font-size: 30px;
    color: $green;
  }
  &-title {
    &.bold {
      font-weight: 700;
    }
    line-height: 93px;
    padding-top: 24px;
    font-size: 80px;
    font-weight: 600;
    color: #919191;
    span {
      color: #fff;
    }
  }
  &-btns {
    padding-top: 50px;
  }
}

@media (max-width: 900px) {
  .mobile {
    &-content {
      flex-direction: column;
      .col-6 {
        width: 100%;
      }
    }
    &-link {
      font-size: 20px;
    }
    &-title {
      font-size: 50px;
    }
    &-box {
      min-height: 500px;
    }
  }
}

@media (max-width: 650px) {
  .mobile {
    padding-left: 10px;
    padding-right: 10px;
  }
}
</style>

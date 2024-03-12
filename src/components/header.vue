<template>
  <div class="header">
    <div class="header-title text-center">
      Own your audience. <br />
      <span>So you don't lose them</span>
    </div>
    <div class="header-subscribe">
      <div class="subcribe flex justify-center column items-center">
        <div class="subscribe-title text-center">
          Turn your audience into email and <br />
          text message subscribers.
        </div>
        <div class="subscribe-btns flex">
          <button class="btn big-blue">Get Started Now</button>
          <button class="btn big-gray">View A Demo</button>
        </div>
        <div class="subscribe-bottom flex items-center">
          <img src="@/assets/image/circle.png" alt="" />
          <div class="subscribe-number">1000+</div>
          <div class="subscribe-text">creators have already started</div>
        </div>
      </div>
    </div>
    <div class="header-creators">
      <div class="title text-center">
        Why Creators Love Marico
      </div>
      <div class="header-creators-boxes flex justify-center column">
        <div class="col-3 col-lg-12">
          <div class="header-creators-box">
            <div class="box-title flex items-center justify-center">
              <img src="@/assets/image/smile-1.png" alt="smile" />Reduced
              Anxiety
            </div>
            <div class="box-text text-center">
              Never worry about losing your audience.
            </div>
          </div>
        </div>
        <div class="col-3 col-lg-12">
          <div class="header-creators-box">
            <div class="box-title flex items-center justify-center">
              <img src="@/assets/image/smile-2.png" alt="smile" />Lower Workload
            </div>
            <div class="box-text text-center">
              Just share one link. We'll handle the rest.
            </div>
          </div>
        </div>
        <div class="col-3 col-lg-12">
          <div class="header-creators-box">
            <div class="box-title flex items-center justify-center">
              <img src="@/assets/image/smile-3.png" alt="smile" />More Time
            </div>
            <div class="box-text text-center">
              Spend less time on marketing tools
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
@import "@/assets/styles/color.scss";
.header {
  padding-top: 128px;
  padding-bottom: 162px;
  &-title {
    line-height: 140px;
    font-size: 112px;
    font-weight: 700;
    span {
      background: -webkit-linear-gradient(360deg, #fe6783, #ffbf84);
      background-clip: text;
      -webkit-text-fill-color: transparent;
    }
  }
  &-subscribe {
    padding-top: 136px;
  }
  .subscribe {
    &-title {
      font-size: 40px;
      font-weight: 500;
      line-height: 60px;
    }
    &-btns {
      padding-top: 50px;
      padding-bottom: 21px;
      gap: 26px;
    }
    &-number {
      padding: 0 10px;
      font-size: 25px;
      font-weight: 700;
    }
    &-text {
      font-size: 25px;
      color: $gray;
    }
  }
  &-creators {
    padding-top: 188px;
    &-boxes {
      padding-top: 64px;
      gap: 100px;
      .box-title {
        font-size: 35px;
        font-weight: 600;
        gap: 8px;
      }
      .box-text {
        padding-top: 10px;
        font-size: 22px;
        color: $gray;
      }
    }
  }
}

@media (max-width: 750px) {
  .header {
    &-title {
      font-size: 80px;
      line-height: 100px;
    }
    .subscribe {
      &-title {
        font-size: 30px;
      }
    }
    &-creators {
      .box-title {
        font-size: 28px;
      }
      .box-text {
        font-size: 18px;
      }
    }
  }
}

@media (max-width: 450px) {
  .header-title {
    font-size: 60px;
  }
  .subscribe {
    &-btns {
      display: flex;
      flex-direction: column;
    }
  }
}
</style>

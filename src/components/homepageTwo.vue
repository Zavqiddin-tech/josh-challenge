<template>
  <div class="homepage flex">
    <div class="col-6 col-lg-12">
      <div class="homepage-content">
        <div class="homepage-content-text">Create & Share</div>
        <div class="title">Reach Your Audience <span>Directly.</span></div>
        <ul class="homepage-lists">
          <li class="homepage-list flex items-center">
            <div class="homepage-list-number flex justify-center items-center">
              1
            </div>
            Embed content or create something new to share.
          </li>
          <li class="homepage-list flex items-center">
            <div class="homepage-list-number flex justify-center items-center">
              1
            </div>
            Share content over email, text message or your homepage.
          </li>
        </ul>
        <div class="homepage-btns flex">
          <button class="btn big-blue">Get Started Now</button>
          <button class="btn big-gray">View A Demo</button>
        </div>
      </div>
    </div>
    <div class="col-6 col-lg-12">
      <div class="homepage-img">
        <img src="@/assets/image/homepage-2.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.homepage {
  padding-top: 182px;
  padding-left: 182px;
  padding-bottom: 70px;
  &-content {
    &-text {
      padding-bottom: 80px;
      font-size: 30px;
      font-weight: 500;
    }
    .title {
      max-width: 700px;
    }
  }
  &-lists {
    padding-top: 27px;
  }
  &-list {
    padding-top: 10px;
    gap: 12px;
    &-number {
      width: 33px;
      height: 33px;
      font-size: 18px;
      font-weight: 500;
      border-radius: 50%;
      background-color: #2d2d2d;
    }
  }
  &-btns {
    padding-top: 66px;
    gap: 24px;
    .big-blue {
      padding: 18px 22px;
    }
    .big-gray {
      padding: 18px 22px;
    }
  }
  &-img {
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}

@media (max-width: 750px) {
  .homepage {
    padding-top: 140px;
    padding-left: 0;
    padding-bottom: 70px;
    flex-direction: column;
    &-content {
      &-text {
        padding-bottom: 50px;
        font-size: 30px;
        text-align: center;
        font-weight: 500;
      }
      .title {
        text-align: center;
        max-width: 100%;
      }
    }
    &-lists {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding-top: 27px;
    }
    &-btns {
      margin-bottom: 20px;
      display: flex;
      justify-content: center;
      padding-top: 66px;
      gap: 24px;
    }
  }
}
</style>

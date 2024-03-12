<template>
  <div class="comment">
    <div class="title text-center">Experts Agree</div>
    <div class="comment-img">
      <img src="@/assets/image/comment.png" alt="comment" />
    </div>
  </div>
  <div class="persons flex justify-center items-center">
    <div class="persons-text text-center">
      We've helped over 1,000 creatorsre claim control of their audience.
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss">
.comment {
  padding: 0px 47px;
  padding-top: 30px;
  &-img {
    height: 442px;
    margin-top: 52px;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}
.persons {
  margin-top: 188px;
  height: 799px;
  background-image: url("@/assets/image/bg-persons.png");
  background-size: cover;
  &-text {
    max-width: 1300px;
    font-size: 70px;
    font-weight: 600;
  }
}

@media (max-width: 750px) {
  .persons {
    &-text {
      font-size: 50px;
    }
  }
}
</style>

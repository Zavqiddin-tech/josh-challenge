<template>
  <div class="container">
    <Navbar />
    <Header />
    <Step
      title="Connect Your Content"
      number="1"
      :btn="true"
      subtitle="Bring all of your content together and get a Homepage that automatically updates whenever you create anywhere online."
    />
    <HomepageOne />
    <Step
      title="Share Your Homepage"
      number="2"
      :btn="false"
      subtitle="Share your Wavium homepage link with your followers, and we'll handle the rest."
    />
    <Mobile />
    <Step
      title="Send Emails & Text Messages"
      number="3"
      :btn="false"
      :medium="true"
      subtitle="No more going through a social platform. Reach and engage your audience directly over email and text massage."
    />
    <HomepageTwo />
    <Comment />
    <Setup />
    <Footer />
  </div>
</template>

<script setup>
import Navbar from "@/components/navbar.vue";
import Header from "@/components/header.vue";
import Step from "@/components/step.vue";
import HomepageOne from "@/components/homepageOne.vue";
import Mobile from "@/components/mobile.vue";
import HomepageTwo from "@/components/homepageTwo.vue";
import Comment from "@/components/comment.vue";
import Setup from "@/components/setup.vue"
import Footer from "@/components/footer.vue";
</script>

<style lang="scss">
@import "@/assets/styles/main.scss";
@import "@/assets/styles/color.scss";
.text {
  color: $blue;
}
</style>
./components/homepageOne.vue
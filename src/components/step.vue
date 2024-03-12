<template>
    <div :class="`${medium ? 'step large' : 'step'}`">
        <div class="step-hero text-center">STEP {{ number }}</div>
        <div :class="`${medium ? 'title-medium text-center' : 'title text-center'}`">{{ title }}</div>
        <div class="subtitle text-center">{{ subtitle }}</div>
        <div v-if="btn" class="step-btn flex justify-center">
            <button  class="btn big-gray">View Avaliable Sources</button>
        </div>
    </div>
</template>

<script setup>
const props = defineProps(['title', 'subtitle', 'btn', 'number', 'medium'])
</script>

<style lang="scss" scoped>
@import "@/assets/styles/color.scss";
.step {
    max-width: 930px;
    margin: auto;
    &.large {
        max-width: 1200px;
    }
    &-hero {
        font-size: 25px;
        color: $blue-step;
    }
    &-btn {
        padding-top: 34px;
    }
    .big-gray {
        padding: 24px 38px;
    }
}

@media (max-width: 750px) {
    .step {
    max-width: 930px;
    margin: auto;
    &.large {
        max-width: 1200px;
    }
    &-hero {
        font-size: 25px;
        color: $blue-step;
    }
    &-btn {
        padding-top: 34px;
    }
    .big-gray {
        padding: 24px 38px;
    }
}
}
</style>
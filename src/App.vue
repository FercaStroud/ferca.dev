<template lang="pug">
div
  TheHeader
  main
    Resume
</template>
<script lang="ts">
import TheHeader from "@/components/TheHeader.vue";
import Resume from "@/components/Resume.vue";

export default {
  components: {TheHeader, Resume}
}
</script>

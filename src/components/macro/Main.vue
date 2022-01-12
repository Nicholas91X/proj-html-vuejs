<template>
  <main>
    <BusinessArea/>
    <AboutArea/>
  </main>
</template>

<script>
import BusinessArea from "../sections/BusinessArea.vue";
import AboutArea from "../sections/AboutArea.vue";
export default {
    name: "Main",
    components: {
      BusinessArea,
      AboutArea
    }
}
</script>

<style lang="scss" scoped>

</style>
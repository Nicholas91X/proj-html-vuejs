<template>
  <main>
    <BusinessArea/>
    <AboutArea/>
    <Projects/>
    <Results/>
    <SendMessage/>
  </main>
</template>

<script>
import BusinessArea from "../sections/BusinessArea.vue";
import AboutArea from "../sections/AboutArea.vue";
import Projects from "../sections/Projects.vue";
import Results from "../sections/Results.vue";
import SendMessage from "../sections/SendMessage.vue";
export default {
    name: "Main",
    components: {
      BusinessArea,
      AboutArea,
      Projects,
      Results,
      SendMessage
    }
}
</script>

<style lang="scss" scoped>


</style>
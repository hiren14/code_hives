<template>
  <div class="container">
    <NavigationBar />
    <Team2021Section />
    <Team2022 />
    <FooterSection />
  </div>
</template>

<script>
import NavigationBar from "~/components/NavigationBar";
import Team2021Section from "~/components/Team2021Section";
import FooterSection from "~/components/FooterSection";
import Team2022 from "../components/Team2022.vue";
export default {
  components: {
    NavigationBar,
    Team2021Section,
    Team2022,
    FooterSection,
  },
};
</script>

<style>
.container {
  display: flex;
  flex-direction: column;
}
</style>

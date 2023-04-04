<template>
  <div class="container">
    
    <NavigationBar />
  <div class="form">
      <br />
      <br />
      <br />
  <hr />

  <!--  changed Data sci 03/04 -->
  <iframe class="res" src="https://docs.google.com/forms/d/e/1FAIpQLSciYkrCU_XBBCh80Cz_X5ZBNfOhXyTVd1FeFpMqDTmGVgy9nQ/viewform?embedded=true" width="640" height="1055" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
<ScrollTopVue />
  <ScrollTopArrowVue />
  
</div>
  </div>
</template>

<script>
import NavigationBar from "~/components/NavigationBar";
import FooterSection from "~/components/FooterSection";
import ScrollTopArrowVue from "../components/ScrollTopArrow.vue";
import ScrollTopVue from "../components/ScrollTop.vue";
  export default {
  components: {
    NavigationBar,
    FooterSection,
    ScrollTopArrowVue,
    ScrollTopVue
  },
};
</script>

<style>
.res{
  position:absolute;
}

.container {
  display: flex;
  flex-direction: column;
}
  @media screen and (max-width: 992px) {
          .form{
              height: 700px;
               width: 700px;   
          }
}

.res{
width: 100%;
}
</style>



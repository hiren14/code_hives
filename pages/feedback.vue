<template>
    <div class="container">
      
      <NavigationBar />
    <!-- <div class="form"> -->
        <br />
        <br />
        <br />
    <hr /><div data-tf-widget="jRGUnyRi" data-tf-iframe-props="title=Dive Into Docker Feedback For Day 1" data-tf-medium="snippet" style="width:100%;height:700px;"></div><script src="//embed.typeform.com/next/embed.js"></script>
<ScrollTopVue />
    <ScrollTopArrowVue />


   
    <ScrollTopVue />
    <ScrollTopArrowVue />
    
  </div>
  
  </template>
  
  <script>
  import NavigationBar from "~/components/NavigationBar";
  import FooterSection from "~/components/FooterSection";
  import ScrollTopVue from "../components/ScrollTop.vue";
import ScrollTopArrowVue from "../components/ScrollTopArrow.vue";
  export default {
    components: {
      NavigationBar,
      FooterSection,
      ScrollTopVue,
      ScrollTopArrowVue,
    },
  };
  </script>
  
  <style>
  
  
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
  
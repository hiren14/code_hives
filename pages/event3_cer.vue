
<template>
    <div class="container">
      
      <NavigationBar />
    <div class="form">
        <br />
        <br />
        <br />
    <hr />
    <iframe class="res" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRMcnoAaRzjY-chB6iQZ4iaXTyE0tdDu9K354HhzjF35kuE-oyP-_GZ3eQ-RRalKDO9fCacjmf8clNi/pubhtml?gid=586725158&amp;single=true&amp;widget=true&amp;headers=false"></iframe>
    <ScrollTopVue />
    <ScrollTopArrowVue />
    
  </div>
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
  .res{
    position:absolute;
    height: 100%;
    width: 100%;
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
  
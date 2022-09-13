<template>
    <div class="container">
      
      <NavigationBar />
    <div class="form">
        <br />
        <br />
        <br />
    <hr />

        <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSeFT2Oe9xSS5ehXHoneO56mSbc0_IShCBIaTTkTdEvLZACvTw/viewform?embedded=true" width="640" height="1700" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe></div>
    </div>
  </template>
  
  <script>
  import NavigationBar from "~/components/NavigationBar";
  import FooterSection from "~/components/FooterSection";
  
  export default {
    components: {
      NavigationBar,
      FooterSection,
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
  </style>
  
<template>
  
    <container class = "chart-bremstemperaturen"><ChartBremstemperaturen/></container>
    <div class="auto-titel">Porsche 911</div>
    
    <img
      class="porsche-von-oben"
      alt=""
      src="/png-porsche-von-oben@2x.png"
    />
    
    <img class="dreieck-hr-icon" alt="" src="/dreieck-hr.svg" />
    <img class="dreieck-hl-icon" alt="" src="/dreieck-hl.svg" />
    <img class="dreieck-vr-icon" alt="" src="/dreieck-hr.svg" />
    <img class="dreieck-vl-icon" alt="" src="/dreieck-hl.svg" />
    
    <div class="reifen-hr-value"><RRTempBremse/></div>
    <div class="reifen-hl-value"><RLTempBremse/></div>
    <div class="reifen-vr-value"><FRTempBremse/></div>
    <div class="reifen-vl-value"><FLTempBremse/></div>
    
    <div class="bremsen-header"></div>
  
</template>
<script>
  import { defineComponent } from "vue";
  import FLTempBremse from "../components/FLTempBremse.vue";
  import RLTempBremse from "../components/RLTempBremse.vue";
  import FRTempBremse from "../components/FRTempBremse.vue";
  import RRTempBremse from "../components/RRTempBremse.vue";
  import ChartBremstemperaturen from "../components/ChartBremstemperaturen.vue";

  export default defineComponent({
    name: "Bremsen",
    components: {FLTempBremse, RLTempBremse, FRTempBremse, RRTempBremse, ChartBremstemperaturen },
  });
</script>



<style scoped>

  .auto-titel {
    position: absolute;
    top: 82px;
    left: 666px;
    font-size: var(--font-size-lg);
    font-weight: 600;
    font-family: var(--font-poppins);
    color: #fff;
  }
  .porsche-von-oben {
    position: absolute;
    top: 209px;
    left: 203px;
    width: 435px;
    height: 498px;
    object-fit: cover;
  }
  .dreieck-hr-icon {
    position: absolute;
    top: 558.2px;
    left: 524.6px;
    border-radius: var(--br-xl);
    width: 46.5px;
    height: 15.9px;
  }
  .dreieck-hl-icon {
    position: absolute;
    top: 556.2px;
    left: 267.3px;
    border-radius: var(--br-xl);
    width: 46.5px;
    height: 15.9px;
  }
  .dreieck-vr-icon {
    position: absolute;
    top: 313.2px;
    left: 519.6px;
    border-radius: var(--br-xl);
    width: 46.5px;
    height: 15.9px;
  }
  .dreieck-vl-icon {
    position: absolute;
    top: 311.2px;
    left: 275.3px;
    border-radius: var(--br-xl);
    width: 46.5px;
    height: 15.9px;
  }
  .reifen-hr-value {
    position: absolute;
    top: 547px;
    left: 577px;
    font-weight: 300;
    display: inline-block;
    width: 99px;
    height: 43px;
    color: #fff;
  }
  .reifen-hl-value {
    position: absolute;
    top: 543px;
    left: 168px;
    font-weight: 300;
    display: inline-block;
    width: 99px;
    height: 43px;
    color: #fff;
  }
  .reifen-vr-value {
    position: absolute;
    top: 302px;
    left: 577px;
    font-weight: 300;
    display: inline-block;
    width: 99px;
    height: 43px;
    color: #fff;
  }
  .reifen-vl-value {
    position: absolute;
    top: 298px;
    left: 176px;
    font-weight: 300;
    display: inline-block;
    width: 99px;
    height: 43px;
    color: #fff;
  }
  
  .bremsen-header {
    position: absolute;
    top: 62px;
    left: 174px;
    width: 1064px;
    height: 67px;
    font-size: var(--font-size-2xl);
    font-family: var(--font-poppins);
  }
  
  .chart-bremstemperaturen {
    position: absolute;
    top: 280px;
    left: 700px;
    max-width: 100%; 
    max-height: 100%;
  }
</style>
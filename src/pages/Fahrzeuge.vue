<template>    
    
  
   <div  @click="onPlusClick" class="plus-icon"> <i class='bx bx-plus' ></i></div>
    
    
    <div class="fahrzeug-hinzufuegen-text">{{ $t('Fahrzeuge Hinzufügen') }}</div>
   
<CarouselExample/>

</template>
<script>
  import { defineComponent } from "vue";
  import CarouselExample from "../components/CarouselExample.vue";

  export default defineComponent({
    name: "Fahrzeuge",
    components: { CarouselExample},
    methods: {
      onPlusClick() {
        this.$router.push("/fahrzeughinzufuegen");
      },
    },
  });
</script>
<style scoped>
  .plus-icon {
    position: absolute;
    top: 57%;
    left: 90%;
    width: 85.5px;
    height: 85.5px;
    overflow: hidden;
    cursor: pointer;
    color: #fff;
    font-size: 50px;
  }
  .fahrzeug-hinzufuegen-text {
    position: absolute;
    top: 60%;
    left: 65.76%;
    color: #fff;
  }
</style>
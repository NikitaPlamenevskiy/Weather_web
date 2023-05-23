<script setup>
  import TemperatureBlock from '@/components/TemperatureBlock.vue'
  import Airquality from '@/components/AirqualityBlock.vue'
  import ForecastWeek from '@/components/ForecastWeek.vue'
</script>

<template>
  <div class="content" >
        <TemperatureBlock/>
        <div class="content-right">
            <Airquality/>
            <Airquality/>
            <ForecastWeek/>
        </div>
    </div>
    <router-view/>
</template>


<style lang="scss">
  @import "@/assets/scss/global.scss";
  
  .content{
    max-width: 1090px;
    margin: 0px auto;
    padding-top: 144px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  .content-right{
    width: 578px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }

</style>
<script>
import TemperatureBlock from '@/components/TemperatureBlock.vue'
import Airquality from '@/components/AirqualityBlock.vue'

import axios from 'axios';


const API_KEY = '749e115bf4584cf1baa95404231805';

//Axios get info from weather API
export default {
    data() {
        return {
            posts:{},
            error: {},
        };
    },
    mounted() {
        axios.get(`https://api.weatherapi.com/v1/forecast.json?key=${API_KEY}&q=Астана&days=7&aqi=yes`)
            // .then(repsonse => console.log(repsonse.data.current));
        .then(response => this.posts = response.data)
        .catch(error => cosnole.log(error))
    },

    components: { TemperatureBlock, Airquality }
}
</script>

<template>
    <div class="container">
        <TemperatureBlock/>
        <Airquality/>
        <Airquality/>
    </div>
    
</template>

<style lang="scss" scoped>
    .container{
        display: flex;
        flex-wrap: wrap;
        justify-content:space-between;
    }
</style>
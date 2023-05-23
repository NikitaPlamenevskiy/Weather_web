<script>
import axios from 'axios';

const API_KEY = '749e115bf4584cf1baa95404231805';

//Axios get info from weather API
export default {
    data() {
        return {
            posts:{
            },
            error: {},
        };
    },
    mounted() {
        axios.get(`https://api.weatherapi.com/v1/forecast.json?key=${API_KEY}&q=Астана&days=7&aqi=yes`)
            .then(repsonse => console.log(repsonse.data));
        // .then(response => this.posts = response.data)
        // .catch(error => cosnole.log(error))
    },
}
</script>

<template>
    
</template>

<style lang="scss" scoped>
</style>
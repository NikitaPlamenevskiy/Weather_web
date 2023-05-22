<script>
    import axios from 'axios'

    import API_KEY from '@/Constants.vue'

    export default {
        data(){
            return {
                posts: {},
                errors: []
            }
        },

        async getForecast (){
            try {
                let response = await axios.get(`https://api.weatherapi.com/v1/forecast.json?key=${API_KEY}&q=Астана&days=7&aqi=yes`)
                this.posts = response.data.current
            } catch (error){
                this.errors.push(error);
            }
        },
    }
</script>
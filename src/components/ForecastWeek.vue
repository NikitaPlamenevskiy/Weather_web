<template>
    <div class="container">
        <div class="forecast-for-day">
            <h2 class="forecast-for-day__name">Monaday</h2>
            <img class="forecast-for-day__image" src="@/assets/img/cloudy.png" alt="cloudy">
            <div class="temperature-container">
                <p class="temperature-container__number">21 <sup>°</sup></p>
                <p class="temperature-container__number">18 <sup>°</sup></p>
            </div>
        </div>
        <div class="forecast-for-day">
            <h2 class="forecast-for-day__name">Tuesday</h2>
            <img class="forecast-for-day__image" src="@/assets/img/rainy.png" alt="rainy">
            <div class="temperature-container">
                <p class="temperature-container__number">21<sup>°</sup></p>
                <p class="temperature-container__number">18 <sup>°</sup></p>
            </div>
        </div>
        <div class="forecast-for-day">
            <h2 class="forecast-for-day__name">Wednesday</h2>
            <img class="forecast-for-day__image" src="@/assets/img/cloudy-with-sun.png" alt="cloudy">
            <div class="temperature-container">
                <p class="temperature-container__number">21 <sup>°</sup></p>
                <p class="temperature-container__number">18 <sup>°</sup></p>
            </div>
        </div>
        <div class="forecast-for-day">
            <h2 class="forecast-for-day__name">Thursday </h2>
            <img class="forecast-for-day__image" src="@/assets/img/sunny.png" alt="sunny">
            <div class="temperature-container">
                <p class="temperature-container__number">21 <sup>°</sup></p>
                <p class="temperature-container__number">18 <sup>°</sup></p>
            </div>
        </div>
        <div class="forecast-for-day">
            <h2 class="forecast-for-day__name">Friday</h2>
            <img class="forecast-for-day__image" src="@/assets/img/storm.png" alt="strom">
            <div class="temperature-container">
                <p class="temperature-container__number">21 <sup>°</sup></p>
                <p class="temperature-container__number">18 <sup>°</sup></p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @import "@/assets/scss/mixins/card.scss";
    .container{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        width: 578px;
        padding: 40px 40px;
        border-radius: 10px;
        background-color: var(--backgorund);
    }

    .forecast-for-day{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        color: var(--primary);
        width: 90px;
        height: 100%;
        margin: 0px;
        &__name{
            color: var(--titleColor);
            margin: 0px;
            font-size: 14px;
            line-height: 17px;
        }
        &__image{
            max-width: 64px;
            max-height: 64px;
            margin-top: 16px;
            margin-bottom: 16px;
        }
    }

    .temperature-container{
        display: flex;
        justify-content: space-between;
        width: 55px;
        margin: 0px auto;
        &__number{
            font-weight: 500;
            font-size: 16px;
            line-height: 19px;
            margin: 0px;
        }
    }
</style>
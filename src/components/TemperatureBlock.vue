<script setup>
import backgroundUrl from '@/assets/img/Backgorund_weatherblock.png'
import TemperatureStatisticsBlock from '@/components/TemperatureStatisticsBlock.vue'
</script>

<template>
    <div class="card" :style="{backgroundImage: `url(${backgroundUrl})`}">
        <div class="weather-block">
            <div class="location">
                <img class="location__pin"  src="@/assets/img/pin.png" alt="pin">
                <h2 class="location__name">
                Rio do Sul, SC
                </h2>
            </div>
            <h2 class="temperature">
                18
                <Sup class="temperature__icon">
                    °C 
                </Sup>
            </h2>
        </div>
        <TemperatureStatisticsBlock></TemperatureStatisticsBlock>
    </div>
</template>

<style lang="scss" scoped>
    @import "@/assets/scss/mixins/card.scss";
    .card{
        @include card;
        background-repeat: no-repeat;
        width: 456px;
        height: 438px;
    }
    .weather-block{
        color: var(--primary);
    }
    .temperature{
        margin-bottom: 160px;
        font-size: 88px;
        text-align: center;
        &__icon{
            font-weight: 400;
            font-size: 24px;
            line-height: 29px;
        }
    }
    .location{
        display: flex;
        justify-content: end;
        align-items: center;
        color: var(--titleColor);
        &__name{
            margin: 0px;
            font-size: 14px;
            font-weight: 400;
            text-align: right;
        }
        &__pin{
            width: 20px;
            height: 20px;
        }
    }
</style>
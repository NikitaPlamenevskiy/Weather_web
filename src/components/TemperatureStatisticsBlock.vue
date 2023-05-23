<template>
    <div class="statistics-block">
                <div class="statistics-block__card">
                    <img class="statistics-block__image" src="@/assets/img/weather_1.png" alt="Windy">
                    <div>
                        <p class="statistics-block__name">
                        Wind
                        </p>
                        <p class="statistics-block__value">
                           <b>17</b> km/h
                        </p>
                    </div>
                </div>
                <div class="statistics-block__card">
                    <img class="statistics-block__image" src="@/assets/img/weather_2.png" alt="Windy">
                    <div>
                        <p class="statistics-block__name">
                        Humidity
                        </p>
                        <p class="statistics-block__value">
                           <b>31</b> %
                        </p>
                    </div>
                </div>
                <div class="statistics-block__card">
                    <img class="statistics-block__image" src="@/assets/img/weather_3.png" alt="Windy">
                    <div>
                        <p class="statistics-block__name">
                        Rain
                        </p>
                        <p class="statistics-block__value">
                           <b>40</b> %
                        </p>
                    </div>
                </div>
            </div>
</template>

<style lang="scss" scoped>
    .statistics-block{
        color: var(--secondary);    
        width: 456px;
        display: flex;
        justify-content: space-between;
            &__card{
                display: flex;
                flex-wrap: wrap;
                justify-content: space-around;
                width: 114px;
                max-height: 60px;
                padding-top: 12px;
                padding-bottom: 12px;
                padding-left: 16px;
                padding-right: 16px;
                background-color: rgba(102, 96, 200, 0.6);
                border-radius: 6px;
            }
            &__name{
                margin: 0px;
                font-weight: 400;
                font-size: 12px;
                line-height: 14px;
            }
            &__value{
                margin: 0px;
                font-size: 18px;
                line-height: 22px;
            }
            &__image{
                max-width: 32px;
                max-height: 32px;
            }
        }
</style>
<template>
    <div class="card">
        <div class="aircondition-title">
            <img class="aircondition-title__image"  src="@/assets/img/leaf.png" alt="Leaf">
            <h1 class="aircondition-title__name">Air quality</h1>
        </div>
        <div class="aircondition-quality">
            <h2 class="aircondition-quality__title">
                Normal
            </h2>
            <p class="aircondition-quality__number">
                100
            </p>
        </div>
        <div class="aircondition-info">
            <div class="aircondition-info__container">
                <p class="aircondition-info__number">
                    12.9
                </p>
                <h2 class="aircondition-info__name">
                    PM2.5
                </h2>
            </div>
            <div class="aircondition-info__container">
                <p class="aircondition-info__number">
                    12.9
                </p>
                <h2 class="aircondition-info__name">
                    PM10
                </h2>
            </div>
            <div class="aircondition-info__container">
                <p class="aircondition-info__number">
                    12.9
                </p>
                <h2 class="aircondition-info__name">
                    SO<sub>2</sub>
                </h2>
            </div>
            <div class="aircondition-info__container">
                <p class="aircondition-info__number">
                    12.9
                </p>
                <h2 class="aircondition-info__name">
                    NO<sub>2</sub> 
                </h2>
            </div>
            <div class="aircondition-info__container">
                <p class="aircondition-info__number">
                    21.2
                </p>
                <h2 class="aircondition-info__name">
                   O<sub>3</sub>
                </h2>
            </div>
            <div class="aircondition-info__container">
                <p class="aircondition-info__number">
                    0.78
                </p>
                <h2 class="aircondition-info__name">
                   CO
                </h2>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @import "@/assets/scss/mixins/card.scss";
    .card{
        @include card;
        color: var(--primary);
        width: 253px;
        height: 200px;
        background-color: var(--backgorund);
    }
    .aircondition-title{
        color: var(--titleColor);
        display: flex;
        justify-content: center;
        align-items: center;
        &__name{
            margin: 0px;
            font-style: normal;
            font-weight: 700;
            font-size: 16px;
            line-height: 19px;
            text-align: center;
        }
        &__image{
            width: 20px;
            height: 20px;
        }
    }
    .aircondition-quality{
        max-width: 60px;
        margin: 0px auto;
        margin-top: 32px;
        margin-bottom: 33px;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        &__title{
            color: var(--green);
            margin: 0px;
            font-style: normal;
            font-weight: 700;
            font-size: 18px;
            line-height: 22px;
        }
        &__number{
            margin: 0px;
            margin-top: 4px;
            font-style: normal;
            font-weight: 700;
            font-size: 40px;
            line-height: 48px;
        }
    }
    .aircondition-info{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        &__container{
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            max-width: 36px; 
        }
        &__number{
            margin: 0px;
            font-size: 14px;
            line-height: 17px;
            color: var(--green);
        }
        &__name{
            margin: 0px;
            margin-top: 2px;
            font-weight: 400;
            font-size: 12px;
            line-height: 14px;
        }
    }
</style>
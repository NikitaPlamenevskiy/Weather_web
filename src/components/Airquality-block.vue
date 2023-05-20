<template>
    <div class="card">
        <div class="aircondition-title">
            <img class="aircondition-title__image"  src="@/assets/leaf.png" alt="Leaf">
            <h1 class="aircondition-title__name">Air quality</h1>
        </div>
        <div class="aircondition-quality">
            <h2 class="aircondition-quality__title">
                Normal
            </h2>
            <p class="aircondition-quality__number">
                21
            </p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .card{
        color: var(--primary);
        width: 277px;
        height: 244px;
        background-color: #6D67D0;
    }
    .aircondition-title{
        color: var(--primary);
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
        width: 60px;
        margin: 0px auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        &__title{
            color: #87EBCD;
            margin: 0px;
            font-style: normal;
            font-weight: 700;
            font-size: 18px;
            line-height: 22px;
        }
        &__number{
            margin: 0px;
            font-style: normal;
            font-weight: 700;
            font-size: 40px;
            line-height: 48px;
        }
    }
</style>
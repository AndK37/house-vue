<template>
    <div class="promo">
        <div class="shadow"></div>
        <img class="promo__image" src="img/promo/back.png" alt="">
        <div class="content">
            <div class="top">
                <img class="star" src="img/promo/star.png" alt="">
                <span class="t1">Новая коллекция французских авторов</span>
            </div>
            <div class="mid">
                <p class="t2">Сложно сказать, почему акционеры крупнейших компаний призывают нас к новым свершениям,
                    которые, в
                    свою очередь, должны быть заблокированы в рамках своих собственных рациональных ограничений.
                </p>
                <p class="t2">
                    Принимая во внимание показатели успешности, граница обучения кадров предопределяет высокую
                    востребованность направлений прогрессивного развития.
                </p>
            </div>
            <div class="bot">
                <button class="b">Ознакомиться</button>
            </div>
        </div>

    </div>
</template>

<script>

</script>

<style scoped>
.promo {
    width: 100%;
    max-width: 1440px;
    height: 576px;
    position: relative;
    margin-left: auto;
    margin-right: auto;
    overflow: hidden;
}

.shadow {
    background: rgba(13, 43, 67, 0.8);
    mix-blend-mode: multiply;
    filter: blur(157.5px);
    z-index: 5;
    position: absolute;
    width: 1004px;
    height: 687px;
    left: -238px;
    top: -57px;

}

img {
    height: 100%;
}

.promo__image {
    width: 100%;
    display: flex;
    margin-left: auto;
    margin-right: auto;
}

.content {
    z-index: 10;
    position: absolute;
    height: 574px;
    top: 70px;
    bottom: 70px;
    left: 5vw;

    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    height: 440px;
}

.top {
    display: flex;
    gap: 10px;
}

.t1 {
    display: flex;
    width: 421px;
    height: 80px;

    font-weight: 500;
    font-size: 40px;
    line-height: 100%;

    color: #F4F6F5;
    text-wrap: wrap;
}

.t2 {
    width: 540px;

    font-weight: 500;
    font-size: 18px;
    line-height: 150%;

    color: #FFFFFF;
}

.b {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 20px 60px;
    gap: 6px;
    width: 257px;
    height: 65px;
    background: #EEDB6D;

    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 23px;
    color: #2C2D35;

    border: none;
}

@media (max-width: 576px) {
    .star {
        height: 50px;
    }
    .promo {
        height: 410px;
        padding: 0;
    }
    .content {
        top: 0;
        padding: 30px;
        gap: 0;
        justify-content: inherit;
    }
    .shadow {
        display: none;
    }

    .t1 {
        font-weight: 500;
        font-size: 24px;
        line-height: 100%;
    }

    .t2 {
        width: 100%;
        font-weight: 500;
        font-size: 16px;
        line-height: 140%;
        text-wrap: wrap;
    }
    .mid {
        width: 100%;
    }
    .b {
width: 120px;
height: 21px;

font-weight: 500;
font-size: 18px;
line-height: 21px;

    }
}
</style>

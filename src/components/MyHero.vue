<template>
    <div class="hero">
        <img src="../../public/img/hero/image.png" alt="">
        <div class="t">
            <span class="t1">Реплики картин от<br><span class="t1" style="color: #598d66;">Inc. House</span></span>
            <span class="t2">Высокое качество отрисовки на плотной бумаге или льняном холсте. Редкие произведения,
                доступные
                цены.</span>
            <button>Продукция</button>
        </div>
    </div>
</template>

<script>

</script>

<style scoped>
.hero {
    display: flex;
    max-width: 1110px;
    max-height: 620px;
    height: 43vw;
    align-items: center;
    margin-left: auto;
    margin-right: auto;
    gap: 10px;
    padding-left: 5vw;
    padding-right: 5vw;
}

.t {
    display: flex;
    flex-direction: column;
    gap: 30px;
}

.t1 {
    font-weight: 500;
    /* font-size: 60px; */
    font-size: 60px;
    line-height: 110%;
    color: #2C2D35;
}

.t2 {
    font-weight: 500;
    font-size: 18px;
    line-height: 150%;
    color: #86928B;
    text-wrap: wrap;
}

img {
    height: 100%;
}

button {
    width: 225px;
    height: 65px;

    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 20px 60px;
    gap: 6px;
    border: 1px solid #598D66;
    background-color: #f4f6f5;

    font-weight: 500;
    font-size: 20px;
    line-height: 23px;

    color: #598D66;
    cursor: pointer;
    margin-top: 20px;
}
button:hover {
    background-color: #598d66;
    color: #fff;
}
@media (max-width: 1052px) {
    .t1 {
        font-weight: 500;
        font-size: 40px;
        line-height: 100%;
    }

    .t2 {
        font-weight: 500;
        font-size: 18px;
        line-height: 150%;
    }

    button {
        padding: 20px 60px;
        gap: 6px;
        width: 210px;
        height: 60px;
        margin-top: 10px;
    }
}

@media (max-width: 768px) {
    .hero {
        max-height: 380px;
        min-height: 239px;
    }

    .t {
        gap: 10px;
    }
}

@media (max-width: 650px) {
    .t {
        gap: 0px;
    }

    img {
        display: none;
    }

    .t1 {
        font-weight: 500;
        font-size: 36px;
        line-height: 100%;
    }

    .t2 {
        font-weight: 500;
        font-size: 16px;
        line-height: 150%;
    }

    button {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        padding: 20px 60px;
        gap: 6px;
    }

    .hero {
        padding: 0;
        gap: 10px;
        width: 100%;
    }
}

@media (max-width: 320px) {}
</style>

<template>
    <div class="wrap">
        <div class="header">
            <div class="logo">
                <img src="../../public/img/header/logo.png" alt="" width="35px">
                <span class="title">Ink. House</span>
            </div>
            <div class="nav">
                <span class="nav-item">Репродукции</span>
                <span class="nav-item">Новинки</span>
                <span class="nav-item">О нас</span>
                <img class="cart" src="../../public/img/header/cart.png" alt="" width="24px">
            </div>
        </div>
    </div>

</template>

<script>

</script>

<style scoped>

.wrap {
    width: 100%; 
    background-color: #e1ede6;
}
.header {
    max-width: 1110px;
    height: 100px;
    margin-left: auto;
    margin-right: auto;
    padding-left: 5vw;
    padding-right: 5vw;
    
    display: flex;
    justify-content: space-between;
}

.logo {
    display: flex;
    align-items: center;
}

.title {
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    line-height: 23px;
    color: #598D66;
}

.nav {
    display: flex;
    align-items: center;
    gap: 50px
}

.nav-item {
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 23px;
    color: #2C2D35;
}

@media (max-width: 768px) {
    .header {
        max-width: 690px;

    }

    .title {
        font-style: normal;
        font-weight: 700;
        font-size: 20px;
        line-height: 23px;
    }

    .nav-item {
        font-style: normal;
        font-weight: 500;
        font-size: 18px;
        line-height: 21px;
    }
}

@media (max-width: 576px) {
    .header {
        max-width: 510px;
        flex-direction: column;
        justify-content: space-evenly;
    }

    .logo {
        align-self: center;
    }

    .nav {
        align-self: center;
        border-top: #c3d1c6 1px solid;
        padding-top: 10px;
    }

    .title {
        font-style: normal;
        font-weight: 700;
        font-size: 20px;
        line-height: 23px;
    }

    .nav-item {
        font-style: normal;
        font-weight: 500;
        font-size: 18px;
        line-height: 21px;
    }
}

@media (max-width: 500px) {
    .header {
        max-width: 290px;
        background-color: #f4f6f5;
    }
    .wrap {
        background-color: #f4f6f5;
    }
    .logo {

    }

    .nav {

    }

    .title {
        
    }

    .nav-item {

    }
}
</style>

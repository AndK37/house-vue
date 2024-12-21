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
            <div class="mob">
                <svg @click="side = !side" width="22" height="18" viewBox="0 0 22 18" fill="none"
                    xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M0.6875 16.5625C0.6875 16.3139 0.786272 16.0754 0.962088 15.8996C1.1379 15.7238 1.37636 15.625 1.625 15.625H20.375C20.6236 15.625 20.8621 15.7238 21.0379 15.8996C21.2137 16.0754 21.3125 16.3139 21.3125 16.5625C21.3125 16.8111 21.2137 17.0496 21.0379 17.2254C20.8621 17.4012 20.6236 17.5 20.375 17.5H1.625C1.37636 17.5 1.1379 17.4012 0.962088 17.2254C0.786272 17.0496 0.6875 16.8111 0.6875 16.5625ZM0.6875 9.0625C0.6875 8.81386 0.786272 8.5754 0.962088 8.39959C1.1379 8.22377 1.37636 8.125 1.625 8.125H20.375C20.6236 8.125 20.8621 8.22377 21.0379 8.39959C21.2137 8.5754 21.3125 8.81386 21.3125 9.0625C21.3125 9.31114 21.2137 9.5496 21.0379 9.72541C20.8621 9.90123 20.6236 10 20.375 10H1.625C1.37636 10 1.1379 9.90123 0.962088 9.72541C0.786272 9.5496 0.6875 9.31114 0.6875 9.0625ZM0.6875 1.5625C0.6875 1.31386 0.786272 1.0754 0.962088 0.899588C1.1379 0.723772 1.37636 0.625 1.625 0.625H20.375C20.6236 0.625 20.8621 0.723772 21.0379 0.899588C21.2137 1.0754 21.3125 1.31386 21.3125 1.5625C21.3125 1.81114 21.2137 2.0496 21.0379 2.22541C20.8621 2.40123 20.6236 2.5 20.375 2.5H1.625C1.37636 2.5 1.1379 2.40123 0.962088 2.22541C0.786272 2.0496 0.6875 1.81114 0.6875 1.5625Z"
                        fill="#4C5866" />
                </svg>

                <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g clip-path="url(#clip0_66445_487)">
                        <path
                            d="M8.24967 20.1667C8.75593 20.1667 9.16634 19.7563 9.16634 19.25C9.16634 18.7438 8.75593 18.3334 8.24967 18.3334C7.74341 18.3334 7.33301 18.7438 7.33301 19.25C7.33301 19.7563 7.74341 20.1667 8.24967 20.1667Z"
                            stroke="#2C2D35" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
                        <path
                            d="M18.3337 20.1667C18.8399 20.1667 19.2503 19.7563 19.2503 19.25C19.2503 18.7438 18.8399 18.3334 18.3337 18.3334C17.8274 18.3334 17.417 18.7438 17.417 19.25C17.417 19.7563 17.8274 20.1667 18.3337 20.1667Z"
                            stroke="#2C2D35" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
                        <path
                            d="M0.916992 0.916626H4.58366L7.04033 13.1908C7.12415 13.6128 7.35374 13.9919 7.68891 14.2617C8.02408 14.5315 8.44346 14.6749 8.87366 14.6666H17.7837C18.2139 14.6749 18.6332 14.5315 18.9684 14.2617C19.3036 13.9919 19.5332 13.6128 19.617 13.1908L21.0837 5.49996H5.50033"
                            stroke="#2C2D35" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
                    </g>
                    <defs>
                        <clipPath id="clip0_66445_487">
                            <rect width="22" height="22" fill="white" />
                        </clipPath>
                    </defs>
                </svg>


            </div>
        </div>
    </div>
    <div v-if="side"
        style="position: fixed; top: 35px; width: 100%; height: 300px; z-index: 100; background-color: #e1ede6;">
        <svg @click="side = !side" style="position: fixed; top: 45px; left: 10px;" width="30" height="30"
            viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path fill-rule="evenodd" clip-rule="evenodd"
                d="M6.75 6.75C6.94891 6.55109 7.2187 6.43934 7.5 6.43934C7.7813 6.43934 8.05109 6.55109 8.25 6.75L23.25 21.75C23.4489 21.9489 23.5606 22.2187 23.5606 22.5C23.5606 22.7813 23.4489 23.0511 23.25 23.25C23.0511 23.4489 22.7813 23.5606 22.5 23.5606C22.2187 23.5606 21.9489 23.4489 21.75 23.25L6.75 8.25C6.55109 8.05109 6.43934 7.7813 6.43934 7.5C6.43934 7.21869 6.55109 6.94891 6.75 6.75Z"
                fill="#2C2D35" />
            <path fill-rule="evenodd" clip-rule="evenodd"
                d="M23.25 6.75C23.4489 6.94891 23.5607 7.2187 23.5607 7.5C23.5607 7.7813 23.4489 8.05109 23.25 8.25L8.25001 23.25C8.0511 23.4489 7.78132 23.5606 7.50001 23.5606C7.21871 23.5606 6.94893 23.4489 6.75002 23.25C6.55111 23.0511 6.43936 22.7813 6.43936 22.5C6.43936 22.2187 6.5511 21.9489 6.75002 21.75L21.75 6.75C21.9489 6.55109 22.2187 6.43934 22.5 6.43934C22.7813 6.43934 23.0511 6.55109 23.25 6.75Z"
                fill="#2C2D35" />
        </svg>
        <div style="display: flex; flex-direction: column; gap: 50px; position: fixed; top: 100px; left: 10px;">
            <span class="t">Репродукции</span>
            <span class="t">Новинки</span>
            <span class="t">О нас</span>
        </div>

    </div>
</template>

<script>
export default {
    data() {
        return {
            side: false,
        }
    }
}
</script>

<style scoped>
.t {
font-weight: 500;
font-size: 18px;
line-height: 21px;
color: #2C2D35;

}
.mob {
    display: none;
}

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

@media (max-width: 320px) {
    .header {
        min-width: 320px;
        background-color: #f4f6f5;
        height: 70px;
        padding: 0;
        margin: 0;

    }

    .wrap {
        background-color: #f4f6f5;
        padding: 0;
    }

    .nav {
        display: none;
    }

    .mob {
        display: flex;
        background-color: #e1ede6;

        justify-content: space-between;
        padding: 15px;
        width: 290px;
    }
}
</style>

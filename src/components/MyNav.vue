<template>
    <div class="nav">
        <div class="n">
            <span>Репродукция</span>
            <div class="items">
                <router-link to="/france">Франция</router-link>
                <router-link to="/germany">Германия</router-link>
                <router-link to="/england">Англия</router-link>
            </div>
        </div>
    </div>

</template>

<script>

</script>

<style scoped>
.nav {
    width: 100%;
}
.n {
    padding-left: 5vw;
    padding-right: 5vw;
    margin-left: auto;
    margin-right: auto;
    max-width: 1100px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.items {
    width: fit-content;
    display: flex;
    gap: 10px;
}

span {
    font-weight: 500;
    font-size: 40px;
    line-height: 110%;
    color: #2C2D35;
}

a {
    padding: 10px 20px;
    background: #D4E8D9;
    border-radius: 20px;
    font-weight: 500;
    font-size: 20px;
    line-height: 23px;
    color: #2C2D35;
    text-decoration: none;
}

a.router-link-exact-active {
    padding: 10px 20px;

    background: #376B44;
    border-radius: 20px;

    font-weight: 500;
    font-size: 20px;
    line-height: 23px;

    color: #F4F6F5;
    text-decoration: none;
}


@media (max-width: 1200px) {
    .n {
        max-width:768px;
    }
}
@media (max-width: 900px) {
    .n {
        max-width:610px;
    }
}
@media (max-width: 678px) {
    .n {
        padding: 0;
        flex-direction: column;
        align-items: flex-start;
        max-width:fit-content;
    }
    span {
        margin-bottom: 10px;
    }
}
@media (max-width: 420px) {
    span {
        font-size: 20px;
    }
    a, a.router-link-exact-active {
        font-size: 14px;
    }
}
</style>

<template>
    <div v-if="country == 'france'" class="list">
        <my-card :image="'img/france/1.png'" :author="'Марсель Руссо'" :title="'Охота Амура'"
            :type="'Холст, масло (50х80)'" :price="'14 500 руб'" />
        <my-card :image="'img/france/2.png'" :author="'Анри Селин'" :title="'Дама с собачкой'"
            :type="'Акрил, бумага (50х80) '" :price="'16 500 руб'" />
        <my-card :image="'img/france/3.png'" :author="'Франсуа Дюпон'" :title="'Процедура'"
            :type="'Цветная литография (40х60) '" :price="'20 000 руб'" />

        <my-card :image="'img/france/4.png'" :author="'Луи Детуш'" :title="'Роза'" :type="'Бумага, акрил (50х80) '"
            :price="'12 000 руб'" />
        <my-card :image="'img/france/5.png'" :author="'Франсуа Дюпон'" :title="'Птичья трапеза'"
            :type="'Цветная литография (40х60) '" :price="'22 500 руб'" />
        <my-card :image="'img/france/6.png'" :author="'Пьер Моранж'" :title="'Пейзаж с рыбой'"
            :type="'Цветная литография (40х60) '" :price="'20 000 руб'" />
    </div>

    <div v-else-if="country == 'germany'" class="list">
        <my-card :image="'img/germany/1.png'" :author="'Курт Вернер'" :title="'Над городом'"
            :type="'Цветная литография (40х60) '" :price="'16 000 руб'" />
        <my-card :image="'img/germany/2.png'" :author="'Макс Рихтер'" :title="'Птенцы'" :type="'Холст, масло (50х80) '"
            :price="'14 500 руб'" />
        <my-card :image="'img/germany/3.png'" :author="'Мартин Майер'" :title="'Среди листьев'"
            :type="'Цветная литография (40х60) '" :price="'20 000 руб'" />

        <my-card :image="'img/germany/4.png'" :author="'Герман Беккер'" :title="'Яркая птица'"
            :type="'Цветная литография (40х60) '" :price="'13 000 руб'" />
        <my-card :image="'img/germany/5.png'" :author="'Вульф Бауэр'" :title="'Дятлы'" :type="'Бумага, акрил (50х80) '"
            :price="'20 000 руб'" />
        <my-card :image="'img/germany/6.png'" :author="'Вальтер Хартманн'" :title="'Большие воды'"
            :type="'Бумага, акрил (50х80) '" :price="'23 000 руб'" />
    </div>

    <div v-else-if="country == 'england'" class="list">
        <my-card :image="'img/england/1.png'" :author="'Пол Смит'" :title="'Дикий зверь'"
            :type="'Акварель, бумага (50х80) '" :price="'19 500 руб'" />
        <my-card :image="'img/england/2.png'" :author="'Джон Уайт'" :title="'Скалистый берег'"
            :type="'Цветная литография (40х60) '" :price="'17 500 руб'" />
        <my-card :image="'img/england/3.png'" :author="'Джим Уотсон'" :title="'Река и горы'"
            :type="'Акварель, бумага (50х80) '" :price="'20 500 руб'" />

        <my-card :image="'img/england/4.png'" :author="'Юджин Зиллион'" :title="'Белый попугай'"
            :type="'Цветная литография (40х60) '" :price="'15 500 руб'" />
        <my-card :image="'img/england/5.png'" :author="'Эрик Гиллман'" :title="'Ночная рыба'"
            :type="'Бумага, акрил (50х80) '" :price="'12 500 руб'" />
        <my-card :image="'img/england/6.png'" :author="'Альфред Барр'" :title="'Рыжий кот'"
            :type="'Цветная литография (40х60) '" :price="'21 000 руб'" />
    </div>
</template>

<script>
import MyCard from '@/components/MyCard.vue'

export default {
    components: {
        "my-card": MyCard,
    },
    props: {
        country: String
    }
}

</script>

<style scoped>
.list {
    margin-left: auto;
    margin-right: auto;
    max-width: 1110px;
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    padding-left: 5vw;
    padding-right: 5vw;
}

@media (max-width: 1250px) {
    .list {
        max-width: 690px;
    }
}

@media (max-width: 766px) {
    .list {
        max-width: 510px;
    }
}

@media (max-width: 567px) {
    .list {
        max-width: 290px;
    }
}
</style>
<template>
    <div class="list">
        <my-card/>
        <my-card/>
        <my-card/>
        <my-card/>
        <my-card/>
        <my-card/>
    </div>
</template>

<script>
import MyCard from '@/components/MyCard.vue'

export default {
  components: {
    "my-card": MyCard,
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
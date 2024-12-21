<template>
  <div class="">
    <card-list :country="'france'" />
  </div>
</template>

<script>
import CardList from '@/components/CardList.vue';
export default {
  components: {
    "card-list": CardList,
  }
}
</script>
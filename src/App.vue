<template>
  <my-header />
  <my-hero />
  <my-nav/>
  <router-view />
  <card-list/>
  <my-promo/>
  <team-desc/>
  <!-- <my-footer/> -->
</template>

<script>
import MyHeader from '@/components/MyHeader.vue'
import MyHero from '@/components/MyHero.vue'
import MyNav from '@/components/MyNav.vue'
import CardList from '@/components/CardList.vue'
import MyPromo from '@/components/MyPromo.vue'
import TeamDesc from '@/components/TeamDesc.vue'
// import MyFooter from '@/components/MyFooter.vue'

export default {
  components: {
    "my-header": MyHeader,
    "my-hero": MyHero,
    "my-nav": MyNav,
    "card-list": CardList,
    "my-promo": MyPromo,
    "team-desc": TeamDesc,
    // "my-footer": MyFooter
  }
}
</script>

<style>
* {
  font-family: 'Raleway';
}

#app {
  background-color: #f4f6f5;
  display: flex;
  gap: 20px;
  flex-direction: column;

}

body {
  margin: 0;
  padding: 0;
}



</style>

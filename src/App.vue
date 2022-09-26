<template>
  <div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'AppVue',
  created() {
    let getItems = localStorage.getItem('setItem')
    if(getItems) {
      return this.$store.commit('GET_ITEMS', JSON.parse(getItems))
    }
  },
}
</script>


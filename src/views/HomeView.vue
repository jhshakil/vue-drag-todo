<template>
  <div>
    <ToDo />
    <items />
  </div>
</template>

<script>
import Items from '@/components/Items.vue'
import ToDo from '../components/ToDo.vue'
export default {
  name: 'HomeView',
  components: {
    ToDo,
    Items,
  }
}
</script>

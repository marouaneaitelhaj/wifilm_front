<script>
import { RouterLink, RouterView } from 'vue-router'
import navbar from '@/components/navbar.vue'
import { mapState } from 'vuex'
export default {
  components: {
    navbar,
  },
}
</script>

<template>
  <navbar />
  <RouterView />
</template>

<style scoped></style>

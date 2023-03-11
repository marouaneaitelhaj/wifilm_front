<script>
import { RouterLink, RouterView } from 'vue-router'
import navbar from '@/components/navbar.vue'
export default {
  data() {
    return {
      token: localStorage.getItem('jwt_token'),
    }
  },
  components: {
    navbar,
  },
  methods: {
    isinvalid() {
      if (localStorage.getItem('jwt_token') !== null) {
        this.$router.push('/')
      }
    },
  },
}
</script>

<template>
  <navbar />
  <RouterView />
</template>

<style scoped></style>

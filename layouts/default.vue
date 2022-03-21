<template>
  <div>
    <nav>ここにナビゲーションバーを入れる</nav>
    <nav-bar />
    <Nuxt />
  </div>
</template>

<script>
import NavBar from '@/components/NavBar.vue';
export default {
  components: {
    NavBar,
  }
}
</script>

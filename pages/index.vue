<template>
  <div class="container">
    <div>
      <NuxtLogo />
      <NuxtTutorial />
      <h1 class="title">Welcome to the Vant + Nuxt.js template</h1>
      <div class="links">
        <van-button> Documentation </van-button>
        <van-button> GitHub </van-button>
        <van-button> Vant UI </van-button>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import NuxtTutorial from '~/components/Tutorial.vue'
export default defineComponent({
  name: 'IndexPage',
  components: {
    NuxtTutorial,
  },
})
</script>
<style lang="less" scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: Quicksand, 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.links {
  padding-top: 15px;
}
</style>

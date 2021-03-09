<template>
  <h1>Login</h1>
  vuex:{{ $store.state.num }}
  <div>
    <button type="primary" @click="goLogin">去首页</button>
  </div>
</template>
<script lang="ts" setup="props">
import { useRouter } from "vue-router";
const router = useRouter();
const goLogin = () => {
  router.push("/");
};
</script>
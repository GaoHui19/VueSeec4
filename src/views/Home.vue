<template>
  <div>
    <h2>首页</h2>
    <div>
      <router-link to="/ref">Ref</router-link>
      <router-link to="/shuxing">shuxing 练习</router-link>
      <router-link to="/xinxi"> xinxi 信息录入 练习</router-link>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
// export default {
//   name: 'Home',
// };
</script>

<style>
div {
  display: flex;
  flex-direction: column;
}
.router-link {
  margin-bottom: 10px;
}
</style>

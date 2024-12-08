<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="login">
    <h2>login</h2>
  </div>
</template>

<script setup lang="ts">
import hyRequest from '../../service'

const name = ['abc', 'cba', 'nba']
name.forEach(function (item) {
  console.log('item', item)
})

hyRequest
  .get({
    url: '/home/multidata',
  })
  .then((res) => {
    console.log(res)
  })
</script>

<style lang="less" scoped>
.login {
  color: palevioletred;
}
</style>

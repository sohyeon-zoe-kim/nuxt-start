<template>
  <div>
    <h1 v-if="error.statusCode === 404">404 페이지</h1>
    <h1 v-else>Error 페이지</h1>
    <p>페이지를 찾을 수 없습니다.</p>
    <NuxtLink to="/">Home으로 돌아가기</NuxtLink>
  </div>
</template>
<script>
export default {
  props: {
    error: {
      type: Object,
      default: () => {},
    },
  },
}
</script>
<style>
</style>
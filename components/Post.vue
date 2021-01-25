<template>
  <img :src='src' alt="" class="inset-0 w-full h-full object-cover mb-4 rounded" />
</template>

<script>
export default {
  name: 'Post',
  props: {
    src: {
      default: '',
    }
  }
}
</script>

<style scoped>

</style>

<template>
  <div class='category relative block'>
    <img src='https://www.w3schools.com/w3css/img_forest.jpg' alt="dsd" class="rounded img" />
    <p class='overlay text-white text-center'>{{ catName }}</p>
  </div>
</template>

<script>
export default {
  name: 'Category',
  props: {
    catName: {
      default: 'Category'
    }
  }
}
</script>

<style scoped>
.category .img{
  width: 230px;
  height: 120px;
}

.category .overlay {
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}


</style>

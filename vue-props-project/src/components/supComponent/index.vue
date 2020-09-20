<template>
  <div class="hello">
      <Children1 msg="你好,这是Children1"></Children1>
      <Children2 msg="你好,这是Children2"></Children2>
  </div>
</template>

<script>
import Children1 from './children1'
import Children2 from './children2'
export default {
  name: "SupComponent",
  components: {
      Children1,
      Children2
  }
};
</script>


<style scoped>

</style>

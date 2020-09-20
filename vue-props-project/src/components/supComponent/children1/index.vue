<template>
  <div class="hello">
      <p>{{msg}}</p>
  </div>
</template>

<script>
export default {
  name: "Children1",
  props: {
    msg: {
        type:String,
        default:""
    }
  },
  mounted () {
    //   this.$parent.$on('fromChild2',msg =>{
    //       console.log(msg);
    //   });
    this.$bus.$on('fromChild2',msg =>{
          console.log(msg);
      });
  },
};
</script>


<style scoped>

</style>

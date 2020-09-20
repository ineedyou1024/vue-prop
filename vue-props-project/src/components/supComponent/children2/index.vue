<template>
  <div class="hello">
      <p>{{msg}}</p>
      <button @click="callChild1">给child1发送信息</button>
  </div>
</template>

<script>
export default {
  name: "Children2",
  props: {
    msg: {
        type:String,
        default:""
    }
  },
  methods: {
      callChild1() {
          //利用事件总线发送信息
          //this.$parent.$emit('fromChild2','来自Child2的问候')
          this.$bus.$emit('fromChild2','来自Child2的问候')
      }
  },
};
</script>


<style scoped>

</style>

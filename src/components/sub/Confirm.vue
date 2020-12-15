<template>
  <div class="confirm-button">
    <button @click="getButtonClick">{{text || '确认'}}</button>
  </div>
</template>

<script>
    export default {
      name: "confirm-button",
      props:["text"],
      data(){
          return{
            msg:"注册成功"
          };
      },
      methods:{
          getButtonClick(){
            this.$emit("message", this.msg);
          }
      }
    }
</script>

<style scoped>

</style>

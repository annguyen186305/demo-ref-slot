<script>
export default {
  name:'demoRef',
  data(){
    return{
    }
  },
  methods:{
    handleClickInputFile(){
      this.$refs.fileInputAvatar.click()
      // console.log();
    }
  }
}
</script>

<template>
  <div class="demo-ref">
    <h1>DemoRef</h1>
    <button
        v-on:click="handleClickInputFile"
        class="avatar">Thay đổi Avatar</button>
    <input
        ref="fileInputAvatar"
        type="file"
        style="display: none;">
</div>
</template>

<style scoped>
.demo-ref{
  margin-top: 100px;
  padding: 100px 30px;
  border: 1px solid black;
}
.avatar {
  color: black;
  border: 2px solid yellow;
  padding: 12px 15px;
  background-color: yellow;
}
.avatar:hover {
  color: red;
  background-color: white;
}
</style>
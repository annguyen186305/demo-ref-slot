<script>
export default {
  name:'tabsComp',
  props:{
    title:String
  },
  data(){
    return{

    }
  },
  methods:{

  }
}
</script>

<template>
  <div class="tabs-comp">
    <div class="tabs-title">
      <span>{{ title }}</span>
      <ion-icon name="heart"></ion-icon>
    </div>
    <div class="tabs-content">
      <slot></slot>
    </div>
  </div>
</template>

<style >
.tabs-title {
  padding: 15px 30px;
  display: flex;
  justify-content: space-between;
  border: 2px solid black;
}
.tabs-content{
  margin-top: 3px;
  padding: 2px;
  border: 2px solid black;
}
.tabs-header {
  margin: 0;
  padding: 0;
  display: flex;
  list-style-type: none;
}
.tabs-header li {
  padding: 8px 15px;
  background-color: olive;
  transition: all .3s ease;
}
.tabs-header li:hover {
  color: white;
  background-color: red;
}
</style>
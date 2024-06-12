<script>


import tabsComp from "@/components/tabsComp.vue";

export default {
  name:'demoSlot',
    components:{
      tabsComp
    },
  data(){
    return{
      tabsHeader:[
        {text: 'Tab1'},
        {text: 'Tab2'},
        {text: 'Tab3'},
      ],
      tabActive:0
    }
  },
  methods:{
    setActiveTab(index){
      console.log('setActiveTab', index);
      this.tabActive = index;
    }
  }
}
</script>

<template>

<div class="demo-slot">
<tabsComp title="Tiêu đề của tab">
  <ul class="tabs-header">
    <li v-for="(item, index) in tabsHeader"
        v-bind:key="index"
        v-on:click="setActiveTab(index)"
    >{{item.text}}</li>
  </ul>
  <div class="tabs-content tab1" v-if="tabActive === 0">
    <p>tab 1 rqffqfzfd2141sffa</p>
  </div>
  <div class="tabs-content tab2" v-if="tabActive === 1">
    <p>tab 2 23523rewgdfbcbc</p>
  </div>
  <div class="tabs-content tab3" v-if="tabActive === 2">
    <p>tab 3 3464574575475474532gdfgchc</p>
  </div>
</tabsComp>
</div>

</template>

<style scoped>
.demo-slot{
  margin-top: 50px;
  padding: 100px 30px;
  border: 1px solid black;
}
</style>
<template>
<div id="app" >
  <div >
    <people :name="item.name" :age="item.age" v-for="item in peoples" :key="item.id" />
  </div>


<!-- <img src="@/assets/logo.png" alt="">
<people name="韩宇琪"></people> -->
</div>
  <!-- <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div> -->
</template>

<script>
// let peophoto=document.getElementById('cmg')
// let photoDom=document.createElement('img')
//     photoDom.className='item.photo'
//     peophoto.appendChild(photoDom)
import people from './people.vue'
// import lemon from './assets/lemon.jpg'
// import jiajia from './assets/2.png'
// import qiqi from './assets/3.png'
// import feifei from './assets/4.jpg'
export default {
  components:{
    people
  },
  data () {
    return {
      peoples:[
        {
          id: 1,
          name:'lemon',
          age:'18',
          photo:'lemon'
        },
        {
          id: 2,
          name:'jiajia',
          age:'17',
          photo:'jiajia'
        },
        {
          id: 3,
          name:'qiqi',
          age:'20',
          photo:'qiqi'
        },
        {
          id: 4,
          name:'feiafei',
          age:'19',
          photo:'feifei'
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

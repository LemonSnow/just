<template>
   <div>
     <!-- <h1>王葳蕤</h1> -->
     <img src="@/assets/2.png" alt="">
     <h1>name:{{name}}</h1> 
     <h4>age:{{age}}</h4>
     </div> 
</template>

<script>
export default {
    props:[
      'name',
      'age'
    ]
    // name="wangning"
}
</script>
<style>

</style>

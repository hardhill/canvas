<template>
  <div class="home">
     <canvas id="game" width="640px" height="400px"/>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'home',
  data:function(){
    return {
      ctx:{}
    }
  },
  calculated:{
    
    
  },
  created:()=>{
    this.Init()
  },
  methods:{
    Init(){
      var ctx = document.getElementById("game").getContext("2d")
      var bg = new Image()
      //var bird = new Image()
      bg.src = "@assets/logo.png"
      ctx.drawImage(bg,0,0)
    }
  }

  
}
</script>
<style scoped>
.home{
  display: block;
  text-align: center;
}
</style>

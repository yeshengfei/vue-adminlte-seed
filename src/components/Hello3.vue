<template>
    <button class="js_click">点我</button>
</template>

<script>
import $ from 'jQuery/jQuery-2.2.0.min';
export default {
  name : 'hello3',
  ready(){
    this.bindClick();
  },
  methods:{
    bindClick(){
      $("body").on("click",".js_click",function(){
        alert("I am jQuery event");
      })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
  .hello {
    h1 {
      color: #42b983;
    }

    .moon {
      color: #ff3300;
    }
  }

</style>

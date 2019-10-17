<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
      <footer class="footer">
      <div class="first" @click="router">
            <img src="../assets/firsth.png" alt="">
            <span>首页</span>
        </div>
     <div class="plan">
            <img src="../assets/planh.png" alt="">
            <span>计划</span>
        </div>
        <div class="trends">
            <img src="../assets/trendsy.png" alt="">
            <span>动态</span>
        </div>
       <div class="myself">
            <img src="../assets/myselfh.png" alt="">
            <span>我的</span>
        </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
/* footer */
footer{
    width: 100%;
    height: 15vw;
    border: 1px RGB(236,236,236) solid;
    background-color: RGB(254,254,254) ;
    position: fixed;
    bottom: 0;
    display: flex;
    justify-content: space-around;
    align-items: center;
}
    footer img{
        width: 6vw;
    }
    footer span{
        font-size: 3vw;
    }
    footer .first,
    footer .plan,
    footer .trends,
    footer .myself{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
</style>

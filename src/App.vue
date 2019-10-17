<template>
  <div id="app">
    <div id="nav">
      <router-link to="/"><img src="./assets/information.png" alt=""></router-link>
      <router-link to="/about"><img src="./assets/add.png" alt=""></router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
    position: absolute;
    width: 100%;
    /* padding: 1vw; */
    height: 10vw;
    display: flex;
    justify-content: space-between;
    align-items: center;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }


    .infor,
    .set{
       width: 50%;
       height: 15vw;
       display: flex;
       align-items: center;
       padding: 4vw;
    }
    .infor img{
         width: 6vw;
    }
    .set{
        display: flex;
        flex-direction: row-reverse;        
    }
    .set img{
        width: 6vw;
        margin-right: 1vw;
        }
}
</style>

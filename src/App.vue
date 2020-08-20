<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>  
     <app-header></app-header>
      <div class="container-fluid"> 
            <el-button type="danger">测试按钮</el-button>
            <div class="row">
                <app-slider></app-slider>
                <div class="col-sm-9 col-sm-offset-3 col-md-10 col-md-offset-2 main">

                </div>
            </div>
        </div>
    <router-view/>

  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
<script>
import AppHeader from '@/components/AppHeader'
import AppSlider from '@/components/AppSlider'
export default {
  name :'app',
  data(){
    return{

    }
  },
  components :{
    AppHeader,AppSlider
  }

}
</script>
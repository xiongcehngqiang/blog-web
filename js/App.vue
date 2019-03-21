<template>
  <div id="app">
    <!-- 公共头部组件 -->

    <Head />
    <!-- 主页大图 -->
    <div class="banner"></div>
    <navBar />
    <el-button @click="visible = true">按钮</el-button>
    <router-view></router-view> <!-- 路由引入的组件将在这里被渲染 -->
  </div>
</template>

<script>
import Head from './components/Head'
import navBar from './components/navBar'
export default {
  data () {
    return {
      msg: 's'
    }
  },
  components: {
    Head,
    navBar
  }
}
</script>

<style lang="scss">
html,
body {
  width: 100%;
  height: 100%;
}
body,
div,
dl,
dt,
dd,
ul,
ol,
li,
h1,
h2,
h3,
h4,
h5,
h6,
pre,
code,
form,
fieldset,
legend,
input,
texarea,
p,
blockquote,
th,
td {
  margin: 0px;
  padding: 0px;
}
#app {
  width: 100%;
  height: 100%;
  .banner {
    width: 100%;
    height: 395px;
    background: url("https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1553739689&di=7e1ce9a30665bb9d4de7c4a268460b2d&imgtype=jpg&er=1&src=http%3A%2F%2Fattimg.dospy.com%2Fimg%2Fday_100221%2F20100221_3895f3db24c21f064c35Q7StqsweChDs.jpg")
      no-repeat center;
    background-size: cover;
  }
}
</style>
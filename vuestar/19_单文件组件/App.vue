<!--
component:组件 目录来统一管理：
src/
  ├── components/        # 放置所有公共组件
  │   └── local.vue
  ├── views/            # 放置页面级组件
  ├── App.vue
  └── main.js

-->


<template>
  <div>
    <own></own>//定义组件
    <hello></hello>
    <ling></ling>
  </div>
</template>

<script>
import own from './components/Own.vue'//引入组件  
import hello from './components/Hello.vue'  
import ling from './components/Ling.vue'

export default {
    name:'App',
    //汇总
    components:{
        own,
        hello,
        ling
    }
}
</script>


<!-- 组件的样式 -->
<style>

</style>
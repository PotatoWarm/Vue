<template>
  <div class="sight">
    <h1>风景名称：{{name}}</h1>
    <h1>风景地址：{{address}}</h1>
    <button @click="showname">点我输出风景名称</button>
  </div>
</template>


<script>
//组件的js(数据、方法)交互代码
//export default sight(定义的名称)  暴露组件  
export default {
    name:'sight',//开发者工具最终呈现的名字为sight
    data(){
        return {
            name:'橘子洲头',
            address:'长沙'
        }
    },
    methods:{
        showname(){
            alert(this.name);
        }
    }
};

//统一暴露
//export {sight};
//默认暴露
//export default sight;

</script>

<!-- 组件(css)的样式 --> 
<style>
.sight{
    background-color:deepskyblue;
}
</style>
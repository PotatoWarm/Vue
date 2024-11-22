    <template>
    <div>
        <h1>风景名称：{{name}}</h1>
        <h1>风景地址：{{address}}</h1>
        <button @click="showname">点我输出风景名称</button>
    </div>
</template>

<script>
export default {
    name:'local',
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
}
</script>

<style>

</style>
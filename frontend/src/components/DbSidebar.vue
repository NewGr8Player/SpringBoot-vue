<template>
    <div>
        <div v-for="it in msg">
            <li name="{{it.url}}" class="el-menu-item is-active" @click="" style="">{{it.text}}</li>
        </div>
    </div>
</template>

<script>

    export default {
        name: 'db-sidebar',
        data() {
            return {
                msg: [{text: 'Dashboard',url: 'xx'},{text: 'Dashboard1',url:'xx1'}]
            }
        },
        methods:{
            liOnClick:function(){
                alert(this.attribute("name"));
            }
        }
    }

</script>

<style>
    li {
        padding-left: 20px;
    }
</style>

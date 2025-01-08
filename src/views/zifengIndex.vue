<template>
    <div>
        <p class="title">index</p>
        <p class="bb">LESS是什么玩意</p>
    </div>
</template>

<script>
export default {
    data(){
        return{
            aaa:'',
        }
    },

    components:{
        //组件
    },
    computed:{

    },
    created(){
        this.getUser();
    },
    methods:{
        getUser(){
            this.axios.post("http://182.61.20.123:3001/singin/match",{
                data:'aaa',
                pwd:'ddd',
            }).then((res) =>{
                console.log(res)
            })
        }
    }
}
</script>

<style lang="less" scoped>

.title{
    font-size: 24px;
}
.bb{
  font-size: @size-16;
  color: @warning-color;
  background: @gray-2;
}
</style>
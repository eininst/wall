<template>
    <div class="page">

        <div class="content bg">
            <div class="iconfont re-align" style="color:#fff1b3">&#xe602;</div>
            <div class="succ-info re-align">提交成功! 感谢您的参与~</div>
           <div @click="find" class="btn01">查看我的作品</div>
            <div v-link="{ path: '/cany1', append: false }" class="btn02">再提交一个</div>
            <p>您的作品将会在3个工作日内进行审核，审核通过后将会发布在活动页面，您可以浏览该作品，或发动您的朋友为您的作品点赞、评论。</p>
            <p>活动期间，您可以凭手机号对作品进行索引和修改，每次修改/补充后，我们会对您的作品进行审核，请耐心等待</p>
        </div>
    </div>
</template>
<script>
    export default {
        data(){
            return {
                tel: ''
            }
        },
        route: {
            data ({ to }) {
                let vm = this;
                vm.tel = to.params.tel;
            }
        },
        methods: {
            find:function(){
                let vm = this;

                vm.$route.router.go({
                    name: 'zuop',
                    params:{
                        tel:vm.tel
                    },
                    append: false
                });

            }
        }
    }
</script>
<style lang="less" scoped>
    input{
        -webkit-appearance:none; /*去除系统默认的样式*/
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);   /* 点击高亮的颜色*/
    }
    input[type="submit"],
    input[type="reset"],
    input[type="button"],
    button { -webkit-appearance: none; }

    textarea {  -webkit-appearance: none;}


    .content
    .iconfont{
        font-size: 4rem;
        color: #fff1b3;
        font-weight: bolder;
        margin-top: 3rem;
    }
    .re-align{
        text-align: center;
    }
    .succ-info{
        color: #fff1b3;
        font-size: 0.8rem;
    }
    .btn01,.btn02{
        margin: 2rem 0.8rem 0 0.8rem;
        border: 0.1rem #fff1b3 solid!important;
        text-align: center;
        font-size: 1rem;
        font-weight: bolder;
        color: #fff1b3;
        /*height: 2.5rem;*/
        line-height: 2.5rem;
    }
    .btn02{
        background: #fff1b3;
        color:red;
        margin-top: 0.5rem;
        margin-bottom: 2rem;
    }
    p{
        margin:0.8rem;
        font-size: 0.7rem;
        color: #fff1b3;
        line-height: 0.8rem;
    }
</style>

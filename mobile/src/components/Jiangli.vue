<template>
    <div class="content-padded myfont">
        <ul>
            <li class="row">
                <div class="col-img">
                    <i><img src="http://www.zhuanti2016.wangziqing.cc/static/wall/pc/imgs/lp_01.jpg"></i>
                </div>
                <div class="col-info">
                    <!--<div class="j-title">入围奖</div>-->
                    <div>所有提交的参评项目，活动结束后都将会通过主办方评审，最终通过评审并认定的项目，都将获得一张“寻找中国幕墙之最”活动官方颁发的徽章及证书，提交者获得纪念徽章和奖品</div>
                </div>
            </li>
            <li class="row">
                <div class="col-img">
                    <i><img src="http://www.zhuanti2016.wangziqing.cc/static/wall/pc/imgs/lp_02.jpg"></i>
                </div>
                <div class="col-info">
                    <!--<div class="j-title">最佳人气奖</div>-->
                    <div>参与项目互动评论，字数超过100字有价值的评论内容，经过组委会审核通过后获得纪念徽章及奖品</div>
                </div>
            </li>
            <li class="row">
                <div class="col-img">
                    <i><img src="http://www.zhuanti2016.wangziqing.cc/static/wall/pc/imgs/lp_03.jpg"></i>
                </div>
                <div class="col-info">
                    <!--<div class="j-title">最佳评论奖</div>-->
                    <div>转发活动至朋友圈并截屏发给活动组，活动期间每个工作日抽取5名发放奖品，每周公布一次获奖名单</div>
                </div>
            </li>

        </ul>
    </div>
</template>
<style lang="less" scoped>
    ul{
        list-style:none;
        padding: 0 0 2rem 0;
        font-size: 0.6rem;
        margin-left: 0.9rem;
        color: #fff;
        line-height: 0.8rem;

    }
    li{
        border-bottom: 0.05rem dotted #fff;
        padding: 0.5rem 0;

    }
    .row i img{
        /*display: block;*/
        width:3.5rem;
        height: 3.5rem;
        border-radius: 50%;
        overflow: hidden;
    }
    .j-title{
        font-size: 0.7rem;
        color: #fff;
        font-weight: bold;
        height: 1.2rem;
        line-height: 1.2rem;
    }
    .col-img{
        width: 25%;
    }
    .col-info{
        width: 75%;
    }
</style>
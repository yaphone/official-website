<template>
    <div id="CompanyIntroduction">
        <div class="banner container-fuild text-center">公司介绍</div>
        <div class="container">
            <div class="row CompanyIntroduction-container">
                <div class="col-xs-12 col-sm-12 col-md-6 wow zoomIn">
                    <img class="img-responsive center-block" src="@/assets/img/zzjg.png">
                </div>
                <div class="col-xs-12 col-sm-12 col-md-6">
                    <h3>开芯原科技有限公司</h3>
                    <p class=".text-justify">公司于2020年10月成立于宁波，是艺科心研究院孵化的公司。随着工程建設和工业设计的人工智能化，中小型设计产业将非常困难得到足够资源来处理这些巨大的数据与负担昂贵的设计工具。开芯原针对这些短板以云服务为基础在各类有关图形图像设计的领域提供颠覆性的解决方案。</p>
                    <p class=".text-justify">1）透过虚拟化计算，渲染资源与人工智能的算法算力，开芯原提供高运算，高智慧，高质量，高速度的工业设计平台，达到每秒70帧的逼真实时渲染。</p>
                    <p class=".text-justify">2）开芯原提供了协同设计的平台，异地的设计师可以轻松的在平台上协同设计提高他们的工作质量与效率。</p>
                    <p class=".text-justify">3）所有的设计数据均保留存储于开芯原平台保证了数据的安全，而数据的共享进而提供了各地设计师们协同设计的基础。</p>
                    <p class=".text-justify">4）地方政府可以在开芯原平台上提供设计工具软件给当地高校与中小企业来共享资源。</p>
                    <p class=".text-justify">5）开芯原的平台可以扶持国内自主研发的工业设计工具。</p>
                </div>
            </div>
            <div class="col-xs-12 col-sm-12 col-md-12 wow zoomIn">
                <img class="img-responsive center-block" src="@/assets/img/hxyw.png">
            </div>
        </div>
    </div>
</template>
<script>
import { WOW } from 'wowjs';
export default {
    name: 'CompanyIntroduction',
    data(){
        return{

        }
    },
    mounted(){
        var wow = new WOW();
        wow.init();
    }
}
</script>
<style scoped>
.banner{
    color: #fff;
    font-size: 30px;
    height: 150px;
    line-height: 150px;
    background-image: url('../assets/img/banner5.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: scroll;
    background-position: center center;
}
.row{
    margin-right: 0;
    margin-left: 0;
}
.CompanyIntroduction-container{
    padding: 100px 0;
    color: #808080;
    transition: all ease 0.5s;
}
.CompanyIntroduction-container>div>p{
    font-size: 14px;
    line-height: 2.5rem;
}
@media screen and (max-width: 997px){
    .CompanyIntroduction-container{
    padding: 10px 0;
    color: #808080;
}
}
</style>


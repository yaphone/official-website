<template>
  <div id="HomePage">
    <!-- 轮播图 -->
    <div id="swiper" class="container-fuild">
      <div class="swiper-container banner-swiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide" v-for="(item,index) in swiperList" :key="index">
            <img class="swiper-lazy" :data-src="item.img" alt="轮播图">
            <!-- <div class="swiper-lazy-preloader"></div>
            <div class="swiper-slide-title">
                <h1>{{item.title}}</h1>
                <p>{{item.content}}</p>
            </div> -->
          </div>
        </div>
        <!-- 如果需要分页器 -->
        <div class="swiper-pagination"></div>

        <!-- 如果需要导航按钮 -->
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>
      </div>
    </div>
    
    <div id="bigData" class="center-block">
      <div style="text-align:center">
        <h2>重点产品</h2>
      </div>
      <div class="row bigData-container">
        <div class="row">
          <div class="col-xs-12 col-sm-12 col-md-3">
            <img class="img-responsive" src="@/assets/img/xinpian.png" alt="芯片研发">
            <h2 class="bigData-title">
              AI芯片研发
              <small>/ AI Chip Development</small>
            </h2>
            <p>开芯原基于RISC-V架构自研NB系列芯片，并提供编译器、操作系统等完整闭环解决方案，为企业提供强大的算力支持。随着人工智能领域不断取得突破性进展。作为实现人工智能技术的重要基石，AI芯片拥有巨大的产业价值和战略地位。作为人工智能产业链的关键环节和硬件基础，AI芯片有着极高的技术研发和创新的壁垒。从芯片发展的趋势来看，现在仍处于AI芯片发展的初级阶段。未来将是AI芯片发展的重要阶段，无论是架构还是设计理念都存在着巨大的创新空间。</p>
          </div>
          <div class="col-xs-12 col-sm-12 col-md-3">
            <img class="img-responsive" src="@/assets/img/cloud2.png" alt="工业设计云">
            <h2 class="bigData-title">
              工业设计云
              <small>/ Industrial Cloud</small>
            </h2>
            <p>开芯原提供了协同设计的工业设计云平台，建设目标是针对我国重点产业，如装备制造及汽车零部件、电子电气等产业的实际需求，构建面向工业产品设计与制造全生命周期管理、工业设计服务生态链的数字化服务平台，为企业特别是中小型企业提供一系列工业产品设计的技术与信息支撑服务，包括工业产品创新设计、工业产品创新设计资源库、工业产品创新设计服务等，以提高产品创新意识和产品设计水平，推进信息化和工业化深度融合。 </p>
            <p></p>
          </div>

          <div class="col-xs-12 col-sm-12 col-md-3">
            <img class="img-responsive" src="@/assets/img/AI_class.png" alt="工业设计云">
            <h2 class="bigData-title">
              智慧课堂
              <small>/ Smart Class</small>
            </h2>
            <p>开芯原基于自研云平台，为宁波本地多所院校提供智慧课堂服务，作为创新教学模式，打破传统的单向教学，实现师生双向互动，是未来教室的首选方案。智慧课堂在“先学后教，以学定教”的教学理念指导下，，利用大数据、云计算、物联网与移动互联等新一代信息技术，最终实现教学内容数字化、教学决策数据化、交流互动多样化、评价反馈及时化、资源推送智能化，促进教师开展精准教学与个性化教学，切实提高教学质量和教学效率。</p>
          </div>

          <div class="col-xs-12 col-sm-12 col-md-3">
            <img class="img-responsive" src="@/assets/img/AI_hosp.png" alt="工业设计云">
            <h2 class="bigData-title">
              AI大健康
              <small>/ AI Great Health</small>
            </h2>
            <p>AI在这次疫情中的表现，让我们看到了人工智能在医疗领域的发展潜力。随着人工智能算力、算法等基础技术条件日渐成熟，政策对发展人工智能技术的大力支持，以及医疗市场数据的不断积累，医疗人工智能将迎来快速发展阶段。</p>
            <p>开芯原结合自身优势，基于NB系统芯片自研算法，利用机器学习和人工智能技术开发了新冠肺炎、血片检测等大健康产品，为多所三甲医院提供服务。</p>
          </div>
        </div>
      </div>
    </div>

    <div class="service">
      <div class="setr">
        <div class="new_gaish_w">
          <h2>解决方案</h2>
          <p>基于人工智能帮助企业成功转型</p>
        </div>
        <div class="service-block">
          <div class="col-md-3 jysf1">
            <img src="./../assets/img/jysf1.png" class="img-responsive center-block" />
            <p class="title2">云计算</p>
            <p class="title3">凭借开芯原NB系列芯片、蓝光海量存储、工业设计云、信息安全技术为客户打造领先的云基础架构。</p>
          </div>
        </div>
        <div class="service-block">
          <div class="col-md-3 jysf1">
            <img src="./../assets/img/gxnfl.png" class="img-responsive center-block" />
            <p class="title2">高性能</p>
            <p class="title3">结合NB系列芯片与人工智能，深入行业应用，定制化开发，激发计算无限潜能。</p>
          </div>
        </div>
        <div class="service-block">
          <div class="col-md-3 jysf1">
            <img src="./../assets/img/aq.png" class="img-responsive center-block" />
            <p class="title2">安全</p>
            <p class="title3">聚焦云数据中心的主机安全，包括操作系统安全、应用安全和数据安全，提供集硬件、操作系统、安全软件“三位一体”的安全方案。</p>
          </div>
        </div>
        <div class="service-block">
          <div class="col-md-3 jysf1">
            <img src="./../assets/img/dsj.png" class="img-responsive center-block" />
            <p class="title2">大数据</p>
            <p class="title3">基于蓝光存储方案，满足数据采集、存储、处理及应用开发大数据基础支撑平台，支撑海量数据规模。</p>
          </div>
        </div>
      </div>
    </div>
    <div id="bigData" class="center-block">
      <div style="text-align:center">
        <h2>成功案例</h2>
      </div>
      <div class="row">
        <div class="row" style="margin: 0 25px">
          <div class="col-xs-12 col-sm-12 col-md-2">
            <img class="img-responsive" src="@/assets/img/maidi.png" alt="迈迪网">
            <h2 class="bigData-title">
              迈迪网
            </h2>
            <p>迈迪网是国内领先的工业零件设计平台，提供工业产品创新设计、工业产品创新设计资源库、工业产品创新设计等服务，汇聚大量设计师在线工作，随着平台的快速发展，迈迪在基础物理设施、设计师协同工作、数据安全等方面遇到问题。</p>
            <p>开芯原基于自研工业设计云，为迈迪网提供完整的解决方案，将业务无缝迁移到云平台，极大地提高了业务能力，解决了迈迪网遇到的问题。</p>
          </div>
          <div class="col-xs-12 col-sm-12 col-md-2">
            <img class="img-responsive" src="@/assets/img/nbdx.png" alt="宁波大学">
            <h2 class="bigData-title">
              宁波大学
            </h2>
            <p>宁波大学是宁波本地重点高校，每年为社会输送大量高素质人才，但传统教学手段越来越难以满足社会发展的需求，尤其是新兴专业如工业设计、数字媒体、人工智能等课程，教学模式亟待更新。</p>
            <p>开芯原立足宁波，服务本地，结合自身优势，为包括宁波大学在内的多所高校提供革命性的教学产品，极大提高了教学质量和学生的学习效率，受到学校领导及社会各届的一致好评。</p>
          </div>
          <div class="col-xs-12 col-sm-12 col-md-2">
            <img class="img-responsive" src="@/assets/img/tkzz.png" alt="太空智造">
            <h2 class="bigData-title">
              太空智造
            </h2>
            <p>太空智造是国内领先的提供建筑设计、结构设计服务的上市公司，伴随着业务的发展，客户对设计模型的要求不断提高，为提高渲染质量，公司不得不快速更新计算设备，虽然运营成本不断增加，但效果依然不够理想。</p>
            <p>开芯原针对太空智造的业务特点，为其专门打造了“工业大脑”，提供强大的CPU、GPU、加速卡等硬件资源和Omniverse等渲染工具，并提供运维服务，运营成本降低的同时，支持了其业务的快速增长。</p>
          </div>
          <div class="col-xs-12 col-sm-12 col-md-2">
            <img class="img-responsive" src="@/assets/img/dxz.png" alt="大西洲">
            <h2 class="bigData-title">
              大西洲
            </h2>
            <p>大西洲是一家提供VR/AR定制开发、三维建模、动画渲染、软硬件系统集成等服务的运营商，疫情期间遇到了远程办公个人PC资源配置低、无法协同工作等诸多问题。</p>
            <p>开芯原依托强大的设计云，提供AnyWhere、AnyTime、AnyDevice的3A服务，在其业务接入设计云后，工程师仅需一部能够上网的设备即可开展设计工作，并可实现多人协同，解决了业务痛点。</p>
          </div>
          <div class="col-xs-12 col-sm-12 col-md-2">
            <img class="img-responsive" src="@/assets/img/zhmsg.png" alt="智慧美术馆">
            <h2 class="bigData-title">
              智慧美术馆
            </h2>
            <p>我国美术馆信息化建设起步较晚，目前仍处于个体独立、封闭式发展状态，不但大量的数字化资源没有进入互联网空间和未能实现信息资源的应用服务，即使进入网络空间的数字化资源也处于孤立状态，数据孤岛现象广泛存在。</p>
            <p>开芯原基于蓝光存储、虚拟现实、人工智能等技术，为艺术品数提供字化存储、沉浸式体验，打造智慧美术馆的样版工程，受到众多艺术家与广大用户的喜爱。</p>
          </div>
          <div class="col-xs-12 col-sm-12 col-md-2">
            <img class="img-responsive" src="@/assets/img/xxg.png" alt="AI血片检测">
            <h2 class="bigData-title">
              血片检测
            </h2>
            <p>人工智能为医疗打开了更大的空间。智慧医疗和AI技术的发展，很大程度上能为医生赋能，为医护工作者带来便利。累积下来的数据与模型，未来则可以整合到更多人机诊疗方案当中，成为智慧医疗生长的基石</p>
            <p>开芯原基于NB系列芯片，自研算法，打造了AI细胞血片检测系统，目前已在多所三甲医院部署运行，成为医护人员的得力助手。</p>
          </div>

        </div>
      </div>
    </div>
    
    <!-- 客户评价 -->
    <div id="customer" class="container-fuild">
      <div class="container customer-container">
        <p class="customer-title text-center">客户评价</p>
        <div class="swiper-container customer-swiper hidden-xs">
          <div class="swiper-wrapper">
            <div
              class="swiper-slide customer-block"
              v-for="(item,index) in customerList"
              :key="index"
            >
              <div class="customer-logo">
                <img class="center-block" :src="item.logo" alt="logo">
              </div>
              <div class="customer-yh">
                <img src="@/assets/img/yinhao.png" alt="引号">
              </div>
              <div class="customer-content1">
                <small>{{item.content}}</small>
              </div>
              <div class="customer-content2">{{item.title}}</div>
            </div>
          </div>
          <!-- 如果需要导航按钮 -->
          <div class="swiper-button-prev"></div>
          <div class="swiper-button-next"></div>
        </div>
        <div class="row visible-xs customer-block">
          <div class="col-xs-12" v-for="(item,index) in customerList" :key="index">
            <div class="customer-logo">
              <img class="center-block" :src="item.logo" alt="logo">
            </div>
            <div class="customer-yh">
              <img src="@/assets/img/yinhao.png" alt="引号">
            </div>
            <div class="customer-content1">
              <small>{{item.content}}</small>
            </div>
            <div class="customer-content2">
              <small>{{item.title}}</small>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- 为什么选择我们 -->
    <div id="whyChooseUs" class="conatiner-fuild">
      <div class="container">
        <div class="whyChooseUs-title text-center">
          <p>为什么选择我们的服务</p>
          <p>THE REASON TO CHOOSING US</p>
        </div>
        <div class="row">
          <div
            class="col-xs-12 col-sm-6 col-md-3 server-wrapper"
            v-for="(item,index) in serverList"
            :key="index"
          >
            <div
              class="server-block wow slideInUp"
              onmouseenter="this.style.color='#28f';this.style.borderColor='#28f'"
              onmouseleave="this.style.color='#666';this.style.borderColor='#ccc'"
            >
              <img class="center-block" :src="item.logo" alt="logo">
              <p class="text-center">{{item.title}}</p>
              <div
                class="text-center"
                v-html="item.content"
                onmouseenter="this.style.color='#28f'"
                onmouseleave="this.style.color='#ccc'"
              ></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- 您身边的IT专家 -->
    <div id="contactUs" class="container-fuild text-center">
      <div class="container contactUs-container wow slideInUp">
        <h1>开芯原</h1>
        <h3>7x24小时提供出色服务</h3>
        <button
          class="btn btn-default btn-sm"
          onmouseleave="this.style.borderColor='#ffffff'; this.style.backgroundColor='#ffffff'; this.style.color='#3f3f3f';"
          onmouseenter="this.style.backgroundColor='transparent'; this.style.borderColor='#ffffff'; this.style.color='#ffffff';"
        >联系我们</button>
        <div class="contactUs-contactWay">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Swiper from "swiper";
import { WOW } from 'wowjs';
export default {
  name: "HomePage",
  data() {
    return {
      swiperList: [
        {
          img: require("@/assets/img/banner1.jpg"),
          path: "",
          title: '',
          content: '',
        },
        {
          img: require("@/assets/img/banner3.jpg"),
          path: "",
          title: '',
          content: '',
        },
        {
          img: require("@/assets/img/banner4.jpg"),
          path: "",
          title: '',
          content: '',
        },
        {
          img: require("@/assets/img/banner7.jpg"),
          path: "",
          title: '',
          content: '',
        }
      ],
      customerList: [
        {
          logo: require("@/assets/img/logo_maidi.png"),
          title:
            "迈迪网设计总监",
          content:
            "目前我们的部分业务运行在开芯原工业设计云上，解决了我们工程师协同工作的难点，提高了工作效率，显著提高了业务承载能力。"
        },
        {
          logo: require("@/assets/img/logo_dxz.png"),
          title:
            "大西洲虚拟现实架构师",
          content:
            "疫情期间我们需要远程办公，但个人PC配置比较低，工程师都在开芯原工业设计云上开展工作，大家协作起来甚至比在公司效率还要高。"
        },
        {
          logo: require("@/assets/img/logo_tk.png"),
          title:
            "太空制造总经理",
          content:
            "开芯原为我们定制开发的工业大脑，不仅为我们提供硬件资源，还解决了配套软件的问题，大大降低了我们的运营成本，为开芯原点赞。"
        },
        {
          logo: require("@/assets/img/logo_nbdx.png"),
          title:
            "宁波大学 宫勇教授",
          content:
            "开芯原的智慧课堂改变了我们的教学方式，现在教师上课比以前方便多了，还可以实时指导生，查看学生作业完成情况，同学们学习效率也大大提高了。"
        },
      ],
      serverList: [
        {
          logo: require("@/assets/img/tel.png"),
          title: "完整解决方案",
          content: "<p>从芯片到软件的全面解决方案</p>让您无后顾之忧"
        },
        {
          logo: require("@/assets/img/computer.png"),
          title: "深入行业",
          content: "<p>深入客户，定制化开发</p>直面客户的业务痛点"
        },
        {
          logo: require("@/assets/img/qq.png"),
          title: "强大团队",
          content: "<p>众多经验丰富的工程师</p>多年开发经验"
        },
        {
          logo: require("@/assets/img/skill.png"),
          title: "完善技术支持",
          content: "<p>由技术支持工程师，负责问题解答</p>需求受理及故障受理"
        }
      ]
    };
  },
  mounted() {
    /* banner-swiper */
    new Swiper(".banner-swiper", {
      loop: true, // 循环模式选项
      effect: 'fade',
      //自动播放
      autoplay: {
        delay: 3000,
        stopOnLastSlide: false,
        disableOnInteraction: false
      },
      // 如果需要分页器
      pagination: {
        el: ".swiper-pagination",
        clickable: true
      },
      // 如果需要前进后退按钮
      navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev"
      },
      // 延迟加载
      lazy: {
        loadPrevNext: true
      },
      observer: true, //修改swiper自己或子元素时，自动初始化swiper
      observeParents: true //修改swiper的父元素时，自动初始化swiper
    });
    /* customer-swiper */
    new Swiper(".customer-swiper", {
      loop: true, // 循环模式选项
      slidesPerView: 3,
      //自动播放
      autoplay: {
        delay: 3000,
        stopOnLastSlide: false,
        disableOnInteraction: false
      },
      // 如果需要前进后退按钮
      navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev"
      },
      observer: true, //修改swiper自己或子元素时，自动初始化swiper
      observeParents: true //修改swiper的父元素时，自动初始化swiper
    });
    /* wowjs动画 */
    var wow = new WOW({
      boxClass: 'wow',
      animateClass: 'animated',
      offset: 0,
      mobile: true,
      live: true
    })
    wow.init();
  }
};
</script>
<style scoped>
/* 整体盒子 */
#HomePage {
  width: 100%;
}

/* 轮播图 */
#swiper {
  height: 600px;
}
#swiper .banner-swiper {
  width: 100%;
  height: 100%;
}
#swiper .banner-swiper .swiper-slide img {
  width: 100%;
  height: 100%;
}
#swiper .banner-swiper .swiper-slide{
  position: relative;
}
#swiper .banner-swiper .swiper-slide-title {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 999999999;
  width: 100%;
  height: 100%;
  color: #fff;
  background: rgba(51, 51, 51, 0.534);
  text-align: center;
  line-height: 80px;
}
#swiper .banner-swiper .swiper-slide-title > h1{
  font-size: 50px;
  margin-top: 12%;
}
#swiper .banner-swiper .swiper-slide-title > p{
  font-size: 20px;
  margin-top: 1%;
  font-weight: 700;
}
/* 大数据管理系统 */
#bigData {
  padding: 10px;
  transition: all ease 0.6s;
  box-sizing: border-box;
}
.bigData-container {
  max-width: 1800px;
  margin:0 auto;
}
#bigData .bigData-title {
  padding-bottom: 10px;
  border-bottom: 1px solid #ccc;
}
#bigData p {
  font-size: 14px;
  color: #333;
  line-height: 2rem;
}
#bigData .bigData-device {
  margin: 50px 0 20px;
}

/* 您身边的IT专家 */
#contactUs {
  color: #fff;
  height: 400px;
  background: url("../assets/img/contact_us_bg.jpg") 0 0 no-repeat;
  background-size: 100% 100%;
  transition: all ease 0.6s;
}
#contactUs .contactUs-container {
  padding-top: 50px;
}
#contactUs .contactUs-container button {
  width: 300px;
  height: 50px;
  margin-top: 40px;
}
#contactUs .contactUs-container .contactUs-contactWay span {
  display: inline-block;
  width: 48px;
  height: 48px;
  margin: 30px;
}
#contactUs .contactUs-container .contactUs-contactWay span:nth-of-type(1) {
  background: url("../assets/img/weixin.png") 0 0 no-repeat;
  background-size: 100% 100%;
}
#contactUs .contactUs-container .contactUs-contactWay span:nth-of-type(2) {
  background: url("../assets/img/weibo.png") 0 0 no-repeat;
  background-size: 100% 100%;
}
#contactUs .contactUs-container .contactUs-contactWay span:nth-of-type(3) {
  background: url("../assets/img/twitter.png") 0 0 no-repeat;
  background-size: 100% 100%;
}

/* 客户评价 */
#customer {
  padding: 50px 0;
  box-sizing: border-box;
  background: #efefef;
  transition: all ease 0.6s;
}
#customer .customer-title {
  font-size: 30px;
  color: rgb(102, 102, 102);
  margin: 0 0 30px;
}
#customer .customer-block {
  background: #fff;
  padding: 30px;
}
#customer .customer-logo img {
  width: 94px;
  height: 94px;
  border: 1px solid #ccc;
}
#customer .customer-yh img {
  width: 34px;
  height: 34px;
}
#customer .customer-content1 {
  padding-bottom: 20px;
  border-bottom: 1px solid #0ce9f1;
}
#customer .customer-content2 {
  padding-top: 20px;
}
/* 为什么选择我们 */
#whyChooseUs {
  padding: 100px;
}
#whyChooseUs .whyChooseUs-title {
  margin-bottom: 50px;
}
#whyChooseUs .whyChooseUs-title p:nth-of-type(1) {
  font-size: 25px;
  font-weight: 500;
}
#whyChooseUs .whyChooseUs-title p:nth-of-type(2) {
  font-size: 14px;
}
#whyChooseUs .server-block {
  padding: 50px 20px;
  border: 1px solid #ccc;
  border-bottom: 5px solid #ccc;
}
#whyChooseUs .server-block img {
  width: 48px;
  height: 48px;
}
#whyChooseUs .server-block > p {
  font-size: 20px;
  margin: 30px 0;
}
#whyChooseUs .server-block > div {
  color: #ccc;
}
/* 媒体查询（手机） */
@media screen and (max-width: 768px) {
  #swiper {
    height: 200px;
  }
  #bigData {
    padding: 30px;
  }
  #bigData .bigData-title {
    font-size: 20px;
  }
  #bigData .bigData-device {
    font-size: 20px;
    margin: 10px 0 10px;
  }
  #contactUs {
    height: 200px;
    transition: all ease 0.6s;
  }
  #contactUs .contactUs-container {
    padding-top: 0;
  }
  #contactUs .contactUs-container h1 {
    font-size: 25px;
  }
  #contactUs .contactUs-container h3 {
    font-size: 18px;
  }
  #contactUs .contactUs-container button {
    width: 200px;
    height: 30px;
    margin-top: 20px;
  }
  #contactUs .contactUs-container .contactUs-contactWay span {
    display: inline-block;
    width: 28px;
    height: 28px;
    margin: 10px;
  }
  #customer {
    padding: 30px 0;
    box-sizing: border-box;
    background: #fff;
  }
  #customer .customer-title {
    font-size: 16px;
    font-weight: bold;
  }
  #customer .customer-logo img {
    width: 94px;
    height: 94px;
  }
  #customer .customer-block {
    padding: 30px;
  }
  #customer .customer-block > div {
    padding: 30px 0;
  }
  #whyChooseUs {
    padding: 20px 0;
    transition: all ease 0.6s;
  }
  #whyChooseUs .whyChooseUs-title p:nth-of-type(1) {
    font-size: 20px;
    font-weight: 700;
  }
  #whyChooseUs .whyChooseUs-title p:nth-of-type(2) {
    font-size: 12px;
  }
  #whyChooseUs .server-block {
    padding: 50px 0;
    border: 1px solid #ccc;
    border-bottom: 5px solid #ccc;
  }
  #whyChooseUs .server-block img {
    width: 48px;
    height: 48px;
  }
  #whyChooseUs .server-block > p {
    font-size: 20px;
    margin: 30px 0;
  }
  #whyChooseUs .server-block > div {
    color: #ccc;
  }
}

/* 媒体查询（平板） */
@media screen and (min-width: 768px) and (max-width: 996px) {
  #swiper {
    height: 400px;
  }
  #bigData {
    padding: 60px;
  }
  #bigData .bigData-title {
    font-size: 30px;
  }
  #bigData .bigData-device {
    font-size: 30px;
    margin: 30px 0 15px;
  }
  #contactUs {
    height: 300px;
  }
  #contactUs .contactUs-container {
    padding-top: 50px;
  }
  #contactUs .contactUs-container h1 {
    font-size: 30px;
  }
  #contactUs .contactUs-container h3 {
    font-size: 20px;
  }
  #contactUs .contactUs-container button {
    width: 300px;
    height: 50px;
    margin-top: 30px;
  }
  #contactUs .contactUs-container .contactUs-contactWay span {
    display: inline-block;
    width: 32px;
    height: 32px;
    margin: 15px;
  }
  #customer .customer-title {
    font-size: 24px;
  }
  #whyChooseUs {
    padding: 20px 0;
  }
}

.service {
  min-height: 485px;
  margin-top: 0px;
  margin-bottom: 60px;
  background: #b4b5b3 url(../assets/img/solution.jpg) no-repeat center top;
  background-size: cover;
  color: #fff;
  text-align: center;
  padding: 45px 0;
}

.setr {
  max-width: 1200px;
  margin: 0 auto;
}

.new_gaish_w {
  max-width: 1200px;
  margin: 0 auto;
  margin-bottom: 30px;
}

.jjfaTit {
  font-size: 20px;
  margin-bottom: 15px;
  color: #fff;
  font-weight: 500;
  text-align: center;
  display: block;
}

.service-block p {font-size: 14px;line-height: 22px;color: #fff;font-weight: 500;text-align: center;}
.service-block img{max-width: 178px; text-align:center; vertical-align: middle; margin-bottom:20px;}

.title1 {font-size: 28px !important}
.title2 {font-size: 20px !important}
.title3 {font-size: 16px !important;}

.in_zdld {
  max-width: 1200px;
  margin: 0 auto;
  margin-top: 30px;
}

.inzd_tab {
  float: left;
  width: 32%;
  margin-right: 1%;
  background: #f7f7f7;
}


.incp_ld{position: relative; text-align:center;}

</style>


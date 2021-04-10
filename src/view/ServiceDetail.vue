<template>
  <div id="ServiceDetail">
    <div class="banner container-fuild text-center">服务</div>
    <div class="container">
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-md-3" id="myScrollspy">
          <ul class="nav nav-tabs nav-stacked center-block" id="myNav">
            <p>特色服务</p>
            <li
              :class="item.id==id?'active':''"
              v-for="(item,index) in serviceNavList"
              :key="index"
            >
              <a :href="'#'+item.id">{{item.title}}</a>
            </li>
          </ul>
        </div>
        <div class="col-xs-12 col-sm-12 col-md-9 content  wow zoomIn">
          <div class="content-block" v-for="(item,index) in serviceContentList" :key="index">
            <h2 :id="item.id">
              {{item.title}}
              <small>/ {{item.eng_title}}</small>
            </h2>
            <div v-html="item.content"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { WOW } from "wowjs";
export default {
  name: "ServiceDetail",
  data() {
    return {
      id: "section-1",
      serviceNavList: [
        {
          id: "section-1",
          title: "芯片研发"
        },
        {
          id: "section-2",
          title: "工业设计云平台"
        },
        {
          id: "section-3",
          title: "大数据存储"
        },
        {
          id: "section-4",
          title: "人工智能技术支持"
        }
      ],
      serviceContentList: [
        {
          id: "section-1",
          title: "芯片研发",
          eng_title: "Chip Customization Development",
          content:
            "<p>针对您的不同需求，开芯原可向您提供SOC、内存、电源等部件的定制化开发，并提供芯片封装、验证、编译器等完整的解决方案，基于RISC-V的强大架构，可实现IP任意扩展，不受系统结构框架的限制，助力行业客户缩减研发成本，提升生产效率。</p>"
        },
        {
          id: "section-2",
          title: "工业设计云平台",
          eng_title: "Industrial Design Cloud",
          content:
            "<p>开芯原通过强大的硬件资源和完善的软件生态支持，基于虚拟化、人工智能等技术，向您提供强大的算力支持，为您实现高运算、高智慧、高质量、高速度的工业设计平台，降低您的运营成本并提高工作效率。</p>"
        },
        {
          id: "section-3",
          title: "大数据存储",
          eng_title: "Big Data Storage",
          content:
            "<p>开芯原与蓝光专业技术团队易华录集团深度合作，提供大容量、长寿命、低能耗、高安全、模块化的蓝光存储服务以及光磁融合存储服务，兼容性强，即插即用，是企业用户价值数据长期保存、重要数据归档备份的理想产品。</p>"
        },
        {
          id: "section-4",
          title: "人工智能技术支持",
          eng_title: "AI Technology Support",
          content:
            "<p>我们拥有强大的人工智能团队，可与您一起，提高您的创造力、解锁新的可能性、提升您的生产力、增强您的影响力，为您提供更加智能的自动化解决方案，满足您不断变化的业务需求。</p>"
        }
      ]
    };
  },
  mounted() {
    this.id = this.$route.params.id;
    var top = document.getElementById(this.id).offsetTop;
    $(window).scrollTop(top + 300);
    $("#myNav").affix({
      offset: {
        top: 300
      }
    });
    var wow = new WOW();
    wow.init();
  }
};
</script>
<style scoped>
.banner {
  color: #fff;
  font-size: 30px;
  height: 150px;
  line-height: 150px;
  background-image: url("../assets/img/banner_2.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: scroll;
  background-position: center center;
}
ul.nav-tabs {
  width: 200px;
  margin-top: 40px;
  border-radius: 4px;
  background: #fff;
  z-index: 99999;
  border: 1px solid #474747;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.067);
}
ul.nav-tabs li {
  text-align: center;
  margin: 0;
  border-top: 1px solid #474747;
}
ul.nav-tabs p {
  color: #fff;
  font-size: 18px;
  font-weight: bold;
  text-align: center;
  background: #474747;
  margin: 0;
  padding: 10px 0;
}
ul.nav-tabs li:first-child {
  border-top: none;
}
ul.nav-tabs li a {
  margin: 0;
  padding: 8px 16px;
  border-radius: 0;
}
ul.nav-tabs li.active a,
ul.nav-tabs li.active a:hover {
  color: #fff;
  background: #474747;
  border: 1px solid #474747;
}
ul.nav-tabs li:first-child a {
  border-radius: 4px 4px 0 0;
}
ul.nav-tabs li:last-child a {
  border-radius: 0 0 4px 4px;
}
ul.nav-tabs.affix {
  top: 30px;
}
.content-block {
  margin: 50px 0;
}
.content-block > h2 {
  padding: 20px 0;
  border-bottom: 1px solid #ccc;
}
</style>

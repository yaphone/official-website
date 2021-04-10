<template>
  <div id="JobChance">
    <div class="banner container-fuild text-center">工作机会</div>
    <div class="container">
      <div class="JobChance-container wow pulse">
        <h2>JAVA软件工程师</h2>
        <p>岗位职责</p>
        <ol>
          <li>负责公司产品及项目系统的功能开发、代码优化；</li>
          <li>负责项目组人员任务的分配与监督，及时解决项目技术问题；</li>
          <li>参与系统需求分析与设计，并负责完成项目核心代码，接口规范制定，架构设计。</li>
        </ol>
        <p>任职要求</p>
        <ol>
          <li>本科及以上学历，计算机相关专业，2年以上工作经验；</li>
          <li>具有丰富的系统分析与架构设计实践经验，熟悉高性能、高并发、高可用性、高扩展性系统架构设计，能够按照产品的发展对技术进行适当的演进；</li>
          <li>精通JAVA；精通SSM等开源框架并熟悉其实现原理；有Spring Cloud经验优先。</li>
          <li>熟悉MySQL、Redis、MongoDB、RabbitMQ等存储、缓存队列中间件并熟悉其架构搭建；熟悉eclipse，IDEA和GIT等开发工具。</li>
          <li>熟悉Html/JavaScript/Css/Ajax基本的前端开发；</li>
          <li>诚恳、踏实、稳重，具备良好的职业操守，具有良好的团队协作、沟通能力，责任心强。</li>
          <li>有开源项目、个人博客者优先考虑。</li>
        </ol>
        <button class="center-block btn btn-warning btn-lg">投递简历</button>
      </div>

      <div class="JobChance-container wow pulse">
        <h2>前端开发工程师</h2>
        <p>岗位职责</p>
        <ol>
          <li>根据业务需求，负责应用程序的设计、开发工作，撰写相关技术文档；</li>
          <li>承担公共前端框架、组件的设计、开发工作；</li>
          <li>持续跟进应用质量，确保高品质产品的上线并及时响应和解决用户问题；</li>
          <li>通过各种前端技术手段，提高用户体验并满足性能要求；</li>
        </ol>
        <p>任职要求</p>
        <ol>
          <li>本科以上学历，计算机软件或相关专业；</li>
          <li>4年及以上前端开发经验；</li>
          <li>精通HTML5/CSS3，熟悉页面架构和布局，对表现与数据分离，熟练使用less或sass进行前端开发；</li>
          <li>精通JavaScript、Ajax、DOM等前端原生技术，掌握面向对象编程思想，熟悉前端模块化和组件封装；</li>
          <li>熟悉Vue.或React等前端主流框架，熟练掌握Vue全家桶，有完整大型项目经验优先；</li>
          <li>熟悉各种WEB缓存技术,熟悉大型网站构架和性能优化；</li>
          <li>熟悉前端编译和构建工具，有webpack配置实战经验优先；</li>
          <li>熟悉ECharts等图表库，有数据可视化项目经验优先；</li>
          <li>对前端性能优化、安全知识浏览器差异等有深入了解和实践经验；</li>
          <li>有强烈的上进心和求知欲，善于学习和实践，善于沟通和逻辑表达，有强烈的团队意识和执行力；</li>
        </ol>
        <button class="center-block btn btn-warning btn-lg">投递简历</button>
      </div>
    </div>
  </div>
</template>
<script>
import { WOW } from 'wowjs';
export default {
  name: "JobChance",
  data() {
    return {};
  },
  mounted(){
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
.JobChance-container {
  margin: 100px;
  padding: 30px;
  transition: all ease 0.5s;
  border: 1px dashed salmon;
}
.JobChance-container h2{
  color: rgb(255, 102, 19);
  font-weight: bolder;
  text-align: center;
}
.JobChance-container p{
font-size: 20px;
  color: rgb(255, 102, 19);
  font-weight: 700;
}
.JobChance-container ol{
    list-style-type: decimal;
    padding-left: 30px;
}
.JobChance-container ol>li{
    font-size: 14px;
    line-height: 2.7rem;
}
@media screen and (max-width: 997px) {
  .JobChance-container {
    margin: 20px 0;
    padding: 20px;
    border: 1px dashed salmon;
  }
}
</style>


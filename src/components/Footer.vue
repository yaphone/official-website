<template>
  <div id="footer" class="container-fluid">
    <p class="address_tel_fax">
      <span>地址：宁波市鄞州区国际金融中心A座23-25F</span>
    </p>
    <p class="email_wx">
      <span>Tel：0574-66882869 Fax：0574-66882869</span>
    </p>
    <p class="email_wx">
      <span>邮箱：support@kaixinyuan.com</span>
    </p>
    <p class="copy">Copyright &copy; 2020 - 2021 开芯原科技有限公司</p>
  </div>
</template>
<script>
export default {
  name: "Footer",
  data() {
    return {};
  }
};
</script>
<style scoped>
#footer {
  width: 100%;
  height: 100%;
  color: #fff;
  background: #474747;
  overflow: hidden;
  text-align: center;
}
.logo {
  width: 95px;
  height: 45px;
  margin: 50px auto 20px;
}
.title {
  font-size: 25px;
  margin-bottom: 20px;
}
.address_tel_fax {
  color: #d3d3d3;
  font-size: 14px;
  margin: 10px 0;
}
.email_wx {
  color: #d3d3d3;
  font-size: 14px;
}
.copy {
  color: #d3d3d3;
  font-size: 14px;
  margin: 10px 0 10px;
}
@media screen and (max-width: 997px) {
  .title {
    font-size: 20px;
  }
  .address_tel_fax {
    font-size: 12px;
  }
  .email_wx {

  font-size: 12px;
}
.copy {
  font-size: 12px;
  margin: 30px 0 10px;
}
}
</style>


<template>
  <div id="footer" class="container-fluid">
    <p id="contact" class="title">联系我们</p>
    <p class="email_wx">
      <span>电话：0755-6128 8670</span>
    </p>

    <p class="email_wx">
      <span>邮箱：{{config.email}}</span>
    </p>
    <p class="email_wx">
      <span>地址：{{config.address}}</span>
    </p>
    <p class="email_wx">
      <span>网址：www.1000vc.com</span>
    </p>
    <p class="email_wx">
      <span>微信公众号：{{config.wxChatPublic}}</span>
    </p>
    <p class="text-center link">
      <router-link to="/home#home">首页</router-link>
      <router-link to="/home#about">关于一百天使</router-link>
      <router-link to="/home#unicorn">独角兽孵化营</router-link>
      <router-link to="/home#angel">天使投资人实战营</router-link>
      <router-link to="/home#encyclopedia">天使百科</router-link>
      <router-link to="/home#aci">ACI俱乐部</router-link>
      <router-link to="/home#contact">联系我们</router-link>
    </p>
    <p>
      <a style="color: #999999;">COPYRIGHT &copy; 一百天使（深圳）孵化器科技有限公司</a>
    </p>
    <p><a style="color: #999999;" href="https://beian.miit.gov.cn/#/Integrated/index" target="_blank">粤ICP备19146298号</a></p>
  </div>
</template>
<script>
import config from '@/config'
export default {
  name: "Footer",
  data() {
    return {
      config: config
    };
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
  padding: 30px 0;
}
.link a{
  padding: 0 5px;
  color: #999999;
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
  margin: 50px 0 10px;
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


<template>
  <!-- 头部整体盒子 -->
  <div id="header" class="container-fuild" style="position: sticky;top: 0;z-index: 99">
    <!-- 头部顶部 -->
    <!-- 电脑导航 -->
    <div class="header-nav container hidden-xs">
      <!-- 导航logo -->
      <div class="header-nav-logo">
        <img src="@/assets/img/baike.jpg">
      </div>
      <!-- 导航内容 -->
      <ul class="header-nav-wrapper">
        <li
          v-for="(item,index) in navList"
          :key="index"
          :class="index==navIndex?'active':''"
          @click="navClick(index,item.name)"
        >
          <router-link :to="item.path">
            {{item.name}}
            <span v-if="item.children.length>0" class="glyphicon glyphicon-menu-down"></span>
            <i class="underline"></i>
          </router-link>
          <dl v-if="item.children.length>0">
            <dt v-for="(i,n) in item.children" :key="n">
              <router-link :to="i.path">{{i.name}}</router-link>
            </dt>
          </dl>
        </li>
      </ul>
    </div>
    <!-- 手机导航 -->
    <div class="header-nav-m container-fuild visible-xs">
      <div class="header-nav-m-logo">
        <img class="center-block" src="@/assets/img/baike.jpg" alt="logo">
        <div style="position:absolute; right: 5%;top: 50%;transform: translateY(-50%)">
          <div class="icon-switch" @click="menuIcon">
            <span :class="[isShow ? 'icon-switch1' : 'icon-switch4']"></span>
            <span :class="[isShow ? 'icon-switch2' : 'icon-switch5']"></span>
            <span :class="[isShow ? 'icon-switch3' : 'icon-switch6']"></span>
          </div>
        </div>
      </div>
      <div v-show="isShow === false">
        <ul class="menu-ul">
          <li v-for="(item, index) in navList" :key="index" @click="isShow=!isShow">
            <a style="color:#999;" :href='`#${item.path}`'> {{ item.name }}</a>
          </li>
        </ul>
      </div>
      <!-- 导航栏 -->
<!--      <div class="header-nav-m-menu text-center">-->
<!--        {{menuName}}-->
<!--        <div-->
<!--          class="header-nav-m-menu-wrapper"-->
<!--          data-toggle="collapse"-->
<!--          data-target="#menu"-->
<!--          @click="menuClick"-->
<!--        >-->
<!--          <span :class="menuClass"></span>-->
<!--        </div>-->
<!--        &lt;!&ndash; 导航内容 &ndash;&gt;-->
<!--        <ul id="menu" class="header-nav-m-wrapper collapse">-->
<!--          <li-->
<!--            v-for="(item,index) in navList"-->
<!--            :key="index"-->
<!--            :class="index==navIndex?'active':''"-->
<!--            @click="navClick(index,item.name)"-->
<!--            data-toggle="collapse"-->
<!--            data-target="#menu"-->
<!--          >-->
<!--            <router-link :to="item.path">-->
<!--              {{item.name}}-->
<!--              <i class="underline"></i>-->
<!--            </router-link>-->
<!--          </li>-->
<!--        </ul>-->
<!--      </div>-->
    </div>
  </div>
</template>
<script>
import config from '@/config'
export default {
  name: "Header",
  data() {
    return {
      config: config,
      navIndex: sessionStorage.getItem('navIndex') ? sessionStorage.getItem('navIndex') : 0,
      menuName: "首页",
      menuClass: "glyphicon glyphicon-menu-down",
      navList: [
        {
          name: "首页",
          path: "/home#home",
          children: []
        },
        {
          name: "关于一百天使",
          path: "/home#about",
          children: []
        },
        {
          name: "独角兽孵化营",
          path: "/home#unicorn",
          children: []
        },
        {
          name: "天使投资人实战营",
          path: "/home#angel",
          children: []
        },
        {
          name: "天使百科",
          path: "/home#encyclopedia",
          children: []
        },
        {
          name: "ACI俱乐部",
          path: "/home#aci",
          children: []
        },
        {
          name: "联系我们",
          path: "/home#contact",
          children: []
        }
      ],
      isShow: true
    };
  },
  methods: {
    menuIcon() {
      this.isShow = !this.isShow
    },
    navClick(index, name) {
      this.navIndex = index;
      sessionStorage.setItem('navIndex',index)
      this.menuName = name;
    },
    menuClick() {
      if (this.menuClass == "glyphicon glyphicon-menu-down") {
        this.menuClass = "glyphicon glyphicon-menu-up";
      } else {
        this.menuClass = "glyphicon glyphicon-menu-down";
      }
    }
  }
};
</script>
<style scoped>
/* 顶部 */
#header {
  background: #fff;
  transition: all ease 0.6s;
}
#header .header-top {
  height: 50px;
  color: #fff;
  font-size: 12px;
  line-height: 50px;
  background: #fff;
}
/* 顶部的图标 */
#header .header-top span {
  margin: 0 8px;
}
/* 导航栏 */
#header .header-nav {
  height: 110px;
}
/* 导航栏logo */
#header .header-nav .header-nav-logo {
  /*width: 100px;*/
  height: 100%;
  float: left;
  position: relative;
}
/* 导航栏logo图片 */
#header .header-nav .header-nav-logo img {
  /*width: 95px;*/
  height: 45px;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  margin: auto;
}
/* 导航栏 导航容器 */
#header .header-nav-fixed .header-nav-wrapper {
  line-height: 50px;
}
#header .header-nav .header-nav-wrapper {
  line-height: 110px;
  float: right;
  margin: 0;
  max-width: 800px;
}
/* 导航栏 每个导航 */
#header .header-nav .header-nav-wrapper > li {
  float: left;
  margin: 0 15px;
  position: relative;
}
/* 导航栏 每个导航下面的 a 链接 */
#header .header-nav .header-nav-wrapper > li > a {
  color: #000;
  font-size: 15px;
  font-weight: bold;
  padding: 15px 0;
  position: relative;
}
/* 导航栏 每个导航下面的 a 链接的下划线 */
#header .header-nav .header-nav-wrapper > li > a > i {
  display: block;
  position: absolute;
  bottom: -2px;
  left: 50%;
  width: 0;
  height: 2px;
  opacity: 0;
  transition: all 0.6s ease;
  background-color: #1e73be;
}
/* 导航栏 每个导航下面的 a 链接的右侧小三角 */
#header .header-nav .header-nav-wrapper > li > a > span {
  font-size: 12px;
  transition: transform ease 0.5s;
}
/* 导航栏 每个导航下面的 a 链接 鼠标滑上去的样式 */
#header .header-nav .header-nav-wrapper > li > a:hover {
  color: #1e73be;
  text-decoration: none;
}
/* 导航栏 每个导航下面的 a 链接 鼠标滑上去下划线的样式 */
#header .header-nav .header-nav-wrapper > li > a:hover .underline {
  opacity: 1;
  width: 100%;
  left: 0;
}
/* 导航栏 每个导航下面的 a 链接 鼠标滑上去三角标的样式 */
#header .header-nav .header-nav-wrapper > li > a:hover span {
  transform: rotate(180deg);
}
/* 导航栏 每个导航下面的 a 链接 鼠标点击后的样式 */
#header .header-nav .header-nav-wrapper > li.active > a {
  color: #1e73be;
  text-decoration: none;
  border-bottom: 2px solid #1e73be;
}
/* 导航栏 每个导航下面的二级导航容器 */
#header .header-nav .header-nav-wrapper > li > dl {
  display: none;
  position: absolute;
  width: 168px;
  top: 80%;
  left: 0;
  z-index: 999999;
  box-shadow: 0 0 3px 1px #ccc;
  background: #fff;
}
/* 导航栏 每个导航下面的二级导航容器的每个导航 */
#header .header-nav .header-nav-wrapper > li > dl > dt {
  width: 100%;
  padding: 10px;
  border-bottom: 1px solid #ccc;
}
/* 导航栏 每个导航下面的二级导航容器的每个导航 当鼠标滑上时的样式*/
#header .header-nav .header-nav-wrapper > li > dl > dt > a:hover {
  text-decoration: none;
}
/* 导航栏 滑上一级导航显示二级导航 */
#header .header-nav .header-nav-wrapper > li:hover dl {
  display: block;
}
#header .header-nav .header-nav-wrapper > li > dl > dt:hover {
  cursor: pointer;
  background: #ccc;
}
@media screen and (max-width: 997px) {
  #header .header-nav-m {
    position: relative;
  }
  /* 导航栏logo容器 */
  #header .header-nav-m .header-nav-m-logo {
    height: 80px;
    position: relative;
  }
  /* 导航栏logo图片 */
  #header .header-nav-m .header-nav-m-logo img {
    /*width: 150px;*/
    height: 45px;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    margin: auto;
  }
  /* 导航栏  菜单容器 */
  #header .header-nav-m .header-nav-m-menu {
    color: #fff;
    height: 50px;
    font-size: 20px;
    line-height: 50px;
    background: #474747;
    position: relative;
  }
  /* 导航栏 菜单图标 */
  #header .header-nav-m .header-nav-m-menu-wrapper {
    position: absolute;
    top: 50%;
    right: 20px;
    margin-top: -20px;
    width: 50px;
    height: 40px;
    color: #fff;
    z-index: 999999;
    font-size: 12px;
  }
  /* 导航栏 */
  #header .header-nav-m .header-nav-m-wrapper {
    position: absolute;
    top: 50px;
    left: 0;
    width: 100%;
    background: #474747;
    z-index: 9999999;
  }
  /* 导航栏 每个导航 */
  #header .header-nav-m .header-nav-m-wrapper > li {
    height: 40px;
    line-height: 40px;
    border-bottom: 1px solid #ccc;
  }
  /* 导航栏 每个导航下面的 a 链接 */
  #header .header-nav-m .header-nav-m-wrapper > li > a {
    color: #fff;
    font-size: 15px;
    font-weight: bold;
    padding: 15px 0;
    position: relative;
  }
  /* 导航栏 每个导航下面的 a 链接的右侧小三角 */
  #header .header-nav .header-nav-wrapper > li > a > span {
    font-size: 10px;
  }
  .flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .icon-switch {
    width: 30px;
    height: 20px;
    position: relative;
  }
  .icon-switch span {
    background: #000;
    width: 30px;
    height: 3px;
    display: block;
    cursor: pointer;
    transition: all 0.2s;
    position: absolute;
    margin: 0;
    padding: 0;
  }
  .icon-switch1 {
    left: 0;
    top: 0;
  }
  .icon-switch2 {
    top: 50%;
    left: 0;
    transform: translateY(-50%);
  }
  .icon-switch3 {
    left: 0;
    bottom: 0;
  }
  .icon-switch4 {
    display: none!important;
  }
  .icon-switch5 {
    top: 50%;
    left: 0;
    transform: rotate(45deg);
  }
  .icon-switch6 {
    left: 0;
    bottom: 0;
    transform: rotate(-45deg) translate(5px, -5px);
  }
  .menu-ul {
    background: #fff;
  }
  .menu-ul li{
    display: block;
    text-align: center;
    line-height: 40px;
    border-bottom: 1px solid #f5f5f5;
  }
}
</style>

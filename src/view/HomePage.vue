<template>
  <div id="HomePage">
    <!-- 轮播图 -->
    <div id="swiper" class="container-fuild">
      <div class="swiper-container banner-swiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide bg">
            <img class="swiper-lazy swiper-img" :data-src='require("@/assets/img/2.jpg")' alt="轮播图">
            <div class="swiper-lazy-preloader"></div>
            <div class="swiper-slide-title">
              <h3 class="swiper-yellow swiper-slide-h3 swiper-slide-h3Xs">一百天使</h3>
              <p class="swiper-title-p">百里挑十的资本实战擂台运营商</p>
            </div>

            <ul class="swiper-abs swiper-ul">
              <li class="fontWhite">400万天使投资人“抱团投资”的实战营</li>
              <li class="fontWhite">4000万中小微企业争夺“真金白银”投资的赛马场</li>
            </ul>
          </div>

          <div class="swiper-slide bg">
            <img class="swiper-lazy swiper-img" :data-src='require("@/assets/img/1.jpg")' alt="轮播图">
            <div class="swiper-lazy-preloader"></div>
            <div class="swiper-slide-title">
              <h3 class="swiper-slide-h3  swiper-yellow">
                百里挑十<br>
                独角兽孵化营
              </h3>
              <h4 class="swiper-yellow swiper-content-p2" >——火热报名中——</h4>
              <p class="swiper-p">承办城市：深圳赛区（第1期)</p>
              <p class="swiper-p">报名时间：2021年6-8月</p>
              <p class="swiper-p">开营时间：2021年9月</p>

              <div class="swiper-content-button">
                <router-link class="btn btn-lg btn-success" to="/home#unicorn">查看详情</router-link>
                <router-link class="btn btn-lg btn-success" to="/home#contact">我要报名</router-link>
              </div>
            </div>

            <ul class="swiper-abs swiper-ul">
              <li class="fontWhite">每期录取100学员，5天4晚，3轮PK，10强获得100万-3亿元投资</li>
              <li class="fontWhite">你敢来，我敢投，真金白银投资不作秀——</li>
            </ul>
          </div>
        </div>
        <!-- 如果需要分页器 -->
        <div class="swiper-pagination"></div>

      </div>
    </div>
    <!-- Tessai资管系统 -->

    <div id="clients" class="clients">
      <div>
        <h4>服务网络</h4>
      </div>
      <div>
        <ul>
          <li>
            <span class="blue">5000</span>
            <span>上市公司</span>
            <div class="line"></div>
          </li>
          <li>
            <span class="blue">2w</span>
            <span>资本机构</span>
            <div class="line"></div>
          </li>
          <li>
            <span class="blue">400w</span>
            <span>LP</span>
            <div class="line"></div>
          </li>
          <li>
            <span class="blue">4000w</span>
            <span>创始人</span>
          </li>
        </ul>
      </div>
    </div>

    <div style="height: 1px;background: #f5f5f5;width: 85%;margin: 0 auto"></div>

    <div id="bigData" class="container-fuild">
      <div id="about" class="row bigData-container">
        <div class="col-xs-12 col-sm-12 col-md-6 wow zoomIn">
          <video class="width100 img-responsive" controls>
            <source src="http://static.1000vc.cn/media/college/collegeNews/1616661662156/%E5%88%98%E5%86%B0%E4%BA%91.mp4">
            Sorry, your browser doesn't support embedded videos.
          </video>
<!--          <img class="img-responsive" src="@/assets/img/img1.png" alt="Tessai资管系统">-->
        </div>
        <div class="col-xs-12 col-sm-12 col-md-6">
          <h2 class="bigData-title">
            关于一百天使
          </h2>
          <p>一百天使是由百位投资人和上市公司高管联合发起成立的实战型独角兽孵化机构，是中国首个“百里挑十”的资本实战擂台运营商，旨在通过“资本+技术+人脉”赋能方式，助力优秀学员企业加速成长为行业独角兽。</p>
          <p>一百天使运营的《百里挑十.独角兽孵化营》、《百里挑十.天使投资人实战营》，是中国首个“百里挑十”的资本实战擂台，致力于为中国4000万中小微企业提供“100万-3亿元”真金白银的股权融资渠道；为中国400万天使投资人提供“抱团投资”的实战渠道；为项目早期投资人提供“股权变现”的退出渠道。</p>
        </div>
      </div>
    </div>

    <div id="bigData" class="container-fuild" style="background: rgba(158, 158, 158, 0.3)">
      <div class="row bigData-container" id="unicorn">

        <div class="col-xs-12 col-sm-12 col-md-6">
          <h2 class="bigData-title">
            百里挑十.独角兽孵化营
          </h2>
          <p>《百里挑十.独角兽孵化营》被誉为“中国4000万中小微企业争夺真金白银投资的赛马场”：</p>
          <p>每期由4位实战派资本大咖担任导师，各招收25名弟子；100学员历经5天4晚，3轮PK，争夺10个首轮100万-5000万元，1个次轮500万-2.5亿元的投资名额。</p>
        </div>

        <div class="col-xs-12 col-sm-12 col-md-6 wow zoomIn">
          <img class="img-responsive" src="@/assets/img/3.jpg" alt="天使百科">
        </div>
      </div>
    </div>

    <div id="bigData" class="container-fuild">
      <div class="row bigData-container" id="angel">
        <div class="col-xs-12 col-sm-12 col-md-6 wow zoomIn">
          <img class="img-responsive" src="@/assets/img/4.jpg" alt="Tessai资管系统">
        </div>
        <div class="col-xs-12 col-sm-12 col-md-6">
          <h2 class="bigData-title">
            百里挑十.天使投资人实战营
          </h2>
          <p>《百里挑十.天使投资人实战营》是中国400万天使投资人“抱团投资”的实战营：</p>
          <p>每期5天4晚，在四位实战派资本导师的辅导下，从100个候选项目中，遴选出10个优质项目进行合投，大大降低投资风险，提高投资收益。</p>
        </div>
      </div>
    </div>

    <div id="bigData" class="container-fuild" style="background: rgba(158, 158, 158, 0.3)">
      <div class="row bigData-container">

        <div class="col-xs-12 col-sm-12 col-md-6" id="encyclopedia">
          <h2 class="bigData-title">
            天使百科
          </h2>
          <p>天使百科是一百天使为学员提供的在线商机对接平台，旨在通过“技术赋能”方式，解决人与人之间、项目与资本之间、产品与客户之间的信息不对称问题。</p>
          <p>天使百科致力为学员提供一站面向全国5000上市公司、2万资本机构、400万天使投资人、4000万中小微企业“约生意”的渠道，让学员找资金、找项目、找客户，从此不再难！</p>
        </div>

        <div class="col-xs-12 col-sm-12 col-md-6 wow zoomIn">
          <img class="img-responsive" src="@/assets/img/5.jpg" alt="天使百科">
        </div>
      </div>
    </div>
    <!-- 您身边的IT专家 -->
    <div id="contactUs" class="container-fuild">
      <div class="container contactUs-container wow slideInUp" id="aci">
        <h1 class="text-center">ACI俱乐部</h1>
        <div class="col-xs-12 col-sm-12 col-md-12">
          <p>中文全称：“ACI国际商业引荐俱乐部”，英文全称：ANGELS  CLUB  INTERNATIONAL ，在华语地区，也叫”一百天使俱乐部（一百天使生意引荐俱乐部），是一百天使在全球的学生会组织，也是学员之间”互荐商机，成人达己“的线下生意引荐俱乐部。</p>
        </div>
<!--        <button-->
<!--          class="btn btn-default btn-sm"-->
<!--          onmouseleave="this.style.borderColor='#ffffff'; this.style.backgroundColor='#ffffff'; this.style.color='#3f3f3f';"-->
<!--          onmouseenter="this.style.backgroundColor='transparent'; this.style.borderColor='#ffffff'; this.style.color='#ffffff';"-->
<!--          @click="navToContactPage"-->
<!--        >联系我们</button>-->
<!--        <div class="contactUs-contactWay">-->
<!--          <span></span>-->
<!--          <span></span>-->
<!--          <span></span>-->
<!--        </div>-->
      </div>
    </div>
    <!-- 客户评价 -->
    <div id="customer" class="container-fuild" style="background: rgba(158, 158, 158, 0.3)">
      <div class="container customer-container">
        <p class="customer-title text-center">资本天使<small>（排名不分先后）</small></p>
        <!-- 电脑端客户评价 -->
        <div class="swiper-container customer-swiper ">
          <div class="swiper-wrapper">
            <div
              class="swiper-slide customer-block swiper-width"
              v-for="(item,index) in customerList"
              :key="index"
              @click="goLink(item.link)"
            >
              <div class="customer-logo mediaLogo">
                <img class="center-block" :src="item.logo" alt="logo">
              </div>
              <div class="customer-content1 text-center">
                {{item.title}}
              </div>
              <div class="customer-content2 text-center">
                <p class="customer-content2-p">{{item.content1}}</p>
                <p style="color: #999">{{item.content2}}</p>
              </div>
            </div>
          </div>
          <!-- 如果需要导航按钮 -->
        </div>

<!--        <div class="swiper-container customer-swiper3 visible-xs">-->
<!--          <div class="swiper-wrapper">-->
<!--            <div-->
<!--              class="swiper-slide customer-block"-->
<!--              v-for="(item,index) in customerList"-->
<!--              :key="index"-->
<!--              style="width: 400px"-->
<!--            >-->
<!--              <div class="customer-logo2">-->
<!--                <img class="center-block" :src="item.logo" alt="logo">-->
<!--              </div>-->
<!--              <div class="customer-content1 text-center">-->
<!--                {{item.title}}-->
<!--              </div>-->
<!--              <div class="customer-content2 text-center">-->
<!--                <p>{{item.content1}}</p>-->
<!--                <p>{{item.content2}}</p>-->
<!--              </div>-->
<!--            </div>-->
<!--          </div>-->
<!--          &lt;!&ndash; 如果需要导航按钮 &ndash;&gt;-->
<!--          <div class="swiper-button-prev"></div>-->
<!--          <div class="swiper-button-next"></div>-->
<!--        </div>-->
        <!-- 手机端客户评价 -->
<!--        <div class="row visible-xs customer-block">-->
<!--          <div class="col-xs-12" v-for="(item,index) in customerList" :key="index">-->
<!--            <div class="customer-logo">-->
<!--              <img class="center-block" :src="item.logo" alt="logo">-->
<!--            </div>-->
<!--            <div class="customer-yh">-->
<!--              <img src="@/assets/img/yinhao_left.png" alt="引号">-->
<!--            </div>-->
<!--            <div class="customer-content1 text-center">-->
<!--              {{item.title}}-->
<!--            </div>-->
<!--            <div class="customer-content2 text-center">-->
<!--              <p>{{item.content1}}</p>-->
<!--              <p>{{item.content2}}</p>-->
<!--            </div>-->
<!--          </div>-->
<!--        </div>-->
      </div>
    </div>

    <div id="customer" class="container-fuild">
      <div class="container customer-container">
        <p class="customer-title text-center">友情链接</p>
        <div class="swiper-container customer-swiper2">
          <div class="swiper-wrapper">
            <div class="swiper-slide swiperFlex" v-for="(item,index) in linkList" :key="index">
              <a target="_blank" :href="item.link">
                <img style="width: 100%" class="swiper-lazy" :src="item.img" :data-src="item.img" alt="轮播图">
              </a>
            </div>
          </div>
          <!-- 如果需要分页器 -->
          <div class="swiper-pagination"></div>
          <!-- 如果需要导航按钮 -->
        </div>
      </div>
    </div>

<!--    <div id="swiper2" class="container-fuild">-->
<!--      <p class="customer-title text-center">友情链接</p>-->
<!--      <div class="swiper-container customer-swiper2">-->
<!--        <div class="swiper-wrapper">-->
<!--          <div class="swiper-slide swiperFlex" v-for="(item,index) in linkList" :key="index">-->
<!--            <img style="width: 100%" class="swiper-lazy" :src="item.img" :data-src="item.img" alt="轮播图">-->
<!--          </div>-->
<!--        </div>-->
<!--        &lt;!&ndash; 如果需要分页器 &ndash;&gt;-->
<!--        <div class="swiper-pagination"></div>-->
<!--        &lt;!&ndash; 如果需要导航按钮 &ndash;&gt;-->
<!--        <div class="swiper-button-prev"></div>-->
<!--        <div class="swiper-button-next"></div>-->
<!--      </div>-->
<!--    </div>-->
    <!-- 为什么选择我们 -->
<!--    <div id="whyChooseUs" class="conatiner-fuild">-->
<!--      <div class="container">-->
<!--        <div class="whyChooseUs-title text-center">-->
<!--          <p>为什么选择我们的服务</p>-->
<!--          <p>THE REASON TO CHOOSING US</p>-->
<!--        </div>-->
<!--        <div class="row">-->
<!--          <div-->
<!--            class="col-xs-12 col-sm-6 col-md-3 server-wrapper"-->
<!--            v-for="(item,index) in serverList"-->
<!--            :key="index"-->
<!--          >-->
<!--            <div-->
<!--              class="server-block wow slideInUp"-->
<!--              onmouseenter="this.style.color='#28f';this.style.borderColor='#28f'"-->
<!--              onmouseleave="this.style.color='#666';this.style.borderColor='#ccc'"-->
<!--            >-->
<!--              <img class="center-block" :src="item.logo" alt="logo">-->
<!--              <p class="text-center">{{item.title}}</p>-->
<!--              <div-->
<!--                class="text-center"-->
<!--                v-html="item.content"-->
<!--                onmouseenter="this.style.color='#28f'"-->
<!--                onmouseleave="this.style.color='#ccc'"-->
<!--              ></div>-->
<!--            </div>-->
<!--          </div>-->
<!--        </div>-->
<!--      </div>-->
<!--    </div>-->
  </div>
</template>
<script>
import Swiper from "swiper";
import { WOW } from 'wowjs';
export default {
  name: "HomePage",
  computed: {
    bg1() {
      return `background:url('${require("@/assets/img/1.jpg")}')`
    },
    bg2() {
      return `background:url('${require("@/assets/img/2.jpg")}')`
    }
  },
  data() {
    return {
      swiperList: [
        {
          img: require("@/assets/img/1.jpg"),
          path: "",
          title: '一百天使',
          content: '百里挑十的资本实战擂台运营商',
        },
        {
          img: require("@/assets/img/2.jpg"),
          path: "",
          title: `百里挑十 \n 独角兽孵化营 \n 天使投资人实战营`,
          content: '——火热报名中——',
          content2: `承办城市：深圳赛区（第一期\n报名时：2021年7、8月\n开营时间：2021年9月`
        },
      ],
      customerList: [
        {
          logo: require("@/assets/img/user/1.png"),
          title: "陈玮",
          content1: "东方富海",
          content2: "东方富海",
          link: 'http://www.ofcapital.com/ofcweb/cwei/index.jhtml'
        },
        {
          logo: require("@/assets/img/user/2.png"),
          title: "李万寿",
          content1: "协同资本",
          content2: "董事长",
          link: 'http://www.syncapital.com/zh/xietongchuangxinguanli'
        },
        {
          logo: require("@/assets/img/user/3.png"),
          title: "厉伟",
          content1: "松禾资本",
          content2: "创始合伙人",
          link: 'http://www.pinevc.com.cn/teaminfo/26.html'
        },
        {
          logo: require("@/assets/img/user/4.png"),
          title: "罗飞",
          content1: "松禾资本",
          content2: "董事长",
          link: 'http://www.pinevc.com.cn/teaminfo/25.html'
        },
        {
          logo: require("@/assets/img/user/5.png"),
          title: "刘昼",
          content1: "达晨创投",
          content2: "董事长",
          link: 'http://www.fortunevc.com/index/team.html'
        },
        {
          logo: require("@/assets/img/user/6.png"),
          title: "郑伟鹤",
          content1: "同创伟业",
          content2: "董事长",
          link: 'http://www.cowincapital.com.cn/index.php?m=goods&c=index&a=personal&id=1'
        },
        {
          logo: require("@/assets/img/user/7.png"),
          title: "肖水龙",
          content1: "创东方投资",
          content2: "董事长",
          link: 'http://www.cdfcn.com/team/32.html'
        },
        {
          logo: require("@/assets/img/user/8.png"),
          title: "张维",
          content1: "基石资本",
          content2: "董事长",
          link: 'https://stonevc.com/Partner/index.aspx'
        },
        {
          logo: require("@/assets/img/user/9.png"),
          title: "曾李青",
          content1: "德迅投资",
          content2: "董事长",
          link: 'https://www.decentcapital.com/zh/staff/5c3234100f79cbd54b320b03'
        },
        {
          logo: require("@/assets/img/user/10.png"),
          title: "杨向阳",
          content1: "源政投资",
          content2: "董事长",
          link: 'https://www.sohu.com/a/105819390_156988'
        },
        {
          logo: require("@/assets/img/user/11.png"),
          title: "林嘉喜",
          content1: "国金投资",
          content2: "董事长",
          link: 'http://www.theific.com/manages-detail.php?CaseId=6'
        },
        {
          logo: require("@/assets/img/user/12.png"),
          title: "熊钢",
          content1: "澳银资本",
          content2: "董事长",
          link: 'http://www.asbvchina.com/article/16/2.html'
        },
        {
          logo: require("@/assets/img/user/13.png"),
          title: "谢闻栗",
          content1: "前海梧桐并购基金",
          content2: "董事长",
          link: 'http://qhee-ma.com/aboutUsController/teamDetail?teamType=2'
        },
        {
          logo: require("@/assets/img/user/14.png"),
          title: "冯卫东",
          content1: "天图资本",
          content2: "管理合伙人",
          link: 'http://www.tiantu.com.cn/cn/team.aspx?index=1&page=1&id=2'
        },
        {
          logo: require("@/assets/img/user/15.png"),
          title: "白文涛",
          content1: "分享投资",
          content2: "董事长",
          link: 'http://www.sharecapital.cn/team'
        },
        {
          logo: require("@/assets/img/user/16.png"),
          title: "蒋国云",
          content1: "时代伯乐资本",
          content2: "董事长",
          link: 'http://www.timesbole.cn/about/?182.html'
        },
        {
          logo: require("@/assets/img/user/17.png"),
          title: "汤大杰",
          content1: "勤智资本",
          content2: "董事长",
          link: 'http://www.triwise.cn/core'
        },
        {
          logo: require("@/assets/img/user/18.png"),
          title: "傅哲宽",
          content1: "啟赋资本",
          content2: "董事长",
          link: 'http://www.qfvc.cn/teamDetail.page?id=182'
        },
        {
          logo: require("@/assets/img/user/19.png"),
          title: "贾珂",
          content1: "创享资本",
          content2: "创始合伙人",
          link: 'http://www.creationventure.com'
        },
        {
          logo: require("@/assets/img/user/20.png"),
          title: "朱波",
          content1: "追梦者基金",
          content2: "创始合伙人",
          link: 'http://www.dreamchasercapital.com/teachers_view.aspx?TypeId=66&Id=306&Fid=t26:66:26'
        },
        {
          logo: require("@/assets/img/user/21.png"),
          title: "陈文正",
          content1: "前海母基金",
          content2: "总裁",
          link: 'http://www.qhpefof.com/#team'
        },
        {
          logo: require("@/assets/img/user/22.png"),
          title: "吴晓丰",
          content1: "璀璨资本",
          content2: "董事长",
          link: 'http://www.brightvc.com/#section-team'
        },
        {
          logo: require("@/assets/img/user/23.png"),
          title: "熊伟",
          content1: "千乘资本",
          content2: "董事长",
          link: 'http://www.qianshengvc.com'
        },
        {
          logo: require("@/assets/img/user/24.png"),
          title: "贾君新",
          content1: "新恒利达资本",
          content2: "董事长",
          link: 'http://www.cnxhld.com/index.php?m=Picture&a=show&id=1'
        },
        {
          logo: require("@/assets/img/user/25.png"),
          title: "成晓华",
          content1: "凯盈资本",
          content2: "董事长",
          link: 'https://mp.weixin.qq.com/s/GFolTUOeoThMSZdJyVJ2Fw'
        },
        {
          logo: require("@/assets/img/user/26.png"),
          title: "胡浪涛",
          content1: "中美创投",
          content2: "创始合合伙人",
          link: 'http://www.sinousvc.com/team'
        },
        {
          logo: require("@/assets/img/user/28.png"),
          title: "刘俊宏",
          content1: "东方赛富资本",
          content2: "董事长",
          link: 'http://www.junsancapital.com/about.html#1'
        },
        {
          logo: require("@/assets/img/user/27.png"),
          title: "廖梓君",
          content1: "君盛投资",
          content2: "董事长",
          link: 'http://www.junsancapital.com/about.html#1'
        },
        {
          logo: require("@/assets/img/user/29.png"),
          title: "张琦",
          content1: "与君资本",
          content2: "董事长",
          link: 'http://yj.lingyuad.cn/'
        },
        {
          logo: require("@/assets/img/user/31.png"),
          title: "邵红霞",
          content1: "达晨财智",
          content2: "合伙人",
          link: 'http://www.fortunevc.com/index/teaminfo/id/244.html'
        },
        {
          logo: require("@/assets/img/user/32.png"),
          title: "易丽君",
          content1: "创享资本",
          content2: "创始合伙人",
          link: 'http://www.creationventure.com'
        },
        {
          logo: require("@/assets/img/user/33.png"),
          title: "秦佩琪",
          content1: "追梦者基金",
          content2: "合伙人",
          link: 'http://www.dreamchasercapital.com/teachers_view.aspx?TypeId=66&Id=309&FId=t26:66:26'
        },
        {
          logo: require("@/assets/img/user/34.png"),
          title: "倪泽望",
          content1: "深创投",
          content2: "董事长",
          link: 'http://www.szvc.com.cn/main/aboutUs/gsgg/index.shtml'
        }
      ],
      serverList: [
        {
          logo: require("@/assets/img/tel.png"),
          title: "核心优势1",
          content: "<p>由专业客服提供人工服务</p>负责疑难问题和故障受理"
        },
        {
          logo: require("@/assets/img/computer.png"),
          title: "核心优势2",
          content: "<p>利用远程视频工具，提供协助</p>帮助客户进行调试、解决故障"
        },
        {
          logo: require("@/assets/img/qq.png"),
          title: "核心优势3",
          content: "<p>利用企业QQ提供在线解答</p>帮助企业快速准确解决问题和故障"
        },
        {
          logo: require("@/assets/img/skill.png"),
          title: "核心优势4",
          content: "<p>由技术支持工程师，负责问题解答</p>需求受理及故障受理"
        }
      ],
      linkList: [
        {
          img: require("@/assets/img/brand/1.jpg"),
          link: 'http://www.qianshengvc.com'
        },
        {
          img: require("@/assets/img/brand/2.png"),
          link: 'http://www.sinousvc.com'
        },
        {
          img: require("@/assets/img/brand/3.png"),
          link: 'http://www.creationventure.com'
        },
        {
          img: require("@/assets/img/brand/4.png"),
          link: 'https://www.tamarace.com'
        },
        {
          img: require("@/assets/img/brand/5.png"),
          link: 'http://www.junsancapital.com'
        },
        {
          img: require("@/assets/img/brand/6.jpg"),
          link: 'http://www.damivc.com'
        },
        {
          img: require("@/assets/img/brand/7.jpg"),
          link: 'http://www.brightvc.com'
        },
        {
          img: require("@/assets/img/brand/8.jpg"),
          link: 'http://www.cnxhld.com'
        },
        {
          img: require("@/assets/img/brand/9.jpg"),
          link: 'http://www.dreamchasercapital.com'
        },
        {
          img: require("@/assets/img/brand/10.jpg"),
          link: 'https://mp.weixin.qq.com/s/FqYO8P5d-VWCAorsQ44h8w'
        },
        {
          img: require("@/assets/img/brand/11.jpg"),
          link: 'http://yj.lingyuad.cn'
        },
        {
          img: require("@/assets/img/brand/12.jpg"),
          link: 'http://www.qfvc.cn'
        },
        {
          img: require("@/assets/img/brand/13.png"),
          link: 'http://www.sharecapital.cn'
        },
        {
          img: require("@/assets/img/brand/14.jpg"),
          link: 'http://qhee-ma.com'
        },
        {
          img: require("@/assets/img/brand/15.png"),
          link: 'http://www.efungcapital.com'
        },
        {
          img: require("@/assets/img/brand/16.jpg"),
          link: 'http://stonevc.com'
        },
        {
          img: require("@/assets/img/brand/17.png"),
          link: 'https://www.decentcapital.com'
        },
        {
          img: require("@/assets/img/brand/18.jpg"),
          link: 'http://www.pinevc.com.cn'
        },
        {
          img: require("@/assets/img/brand/19.png"),
          link: 'http://www.cdfcn.com'
        },
        {
          img: require("@/assets/img/brand/20.jpg"),
          link: 'http://www.fortunevc.com'
        },
        {
          img: require("@/assets/img/brand/21.png"),
          link: 'http://www.ofcapital.com'
        },
        {
          img: require("@/assets/img/brand/22.jpg"),
          link: 'http://www.qhpefof.com'
        },
        {
          img: require("@/assets/img/brand/23.png"),
          link: 'http://www.cowincapital.com.cn'
        },
        {
          img: require("@/assets/img/brand/24.jpg"),
          link: 'http://www.triwise.cn'
        },
        {
          img: require("@/assets/img/brand/25.png"),
          link: 'http://www.theific.com'
        },
        {
          img: require("@/assets/img/brand/26.jpg"),
          link: 'http://www.tiantu.com.cn'
        },
        {
          img: require("@/assets/img/brand/27.jpg"),
          link: 'http://www.syncapital.com'
        },
        {
          img: require("@/assets/img/brand/28.jpg"),
          link: 'http://www.asbvchina.com'
        },
        {
          img: require("@/assets/img/brand/29.jpg"),
          link: 'http://www.szvc.com.cn'
        },
        {
          img: require("@/assets/img/brand/30.jpg"),
          link: 'http://www.timesbole.cn'
        },
      ],
    };
  },
  mounted() {
    /* banner-swiper */
    new Swiper(".banner-swiper", {
      loop: true, // 循环模式选项
      effect: 'fade',
      //自动播放
      autoplay: {
        delay: 6000,
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
      slidesPerView: 4,
      breakpoints: {
        // when window width is >= 320px
        480: {
          slidesPerView: 2
        },
      },
      //自动播放
      autoplay: {
        delay: 6000,
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

    new Swiper(".customer-swiper2", {
      loop: true, // 循环模式选项
      slidesPerView: 6,
      spaceBetween: 50,
      //自动播放
      autoplay: {
        delay: 6000,
        stopOnLastSlide: false,
        disableOnInteraction: false
      },
      breakpoints: {
        // when window width is >= 320px
        480: {
          slidesPerView: 2
        },
      },
      // 如果需要前进后退按钮
      navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev"
      },
      observer: true, //修改swiper自己或子元素时，自动初始化swiper
      observeParents: true //修改swiper的父元素时，自动初始化swiper
    });

    new Swiper(".customer-swiper3", {
      loop: true, // 循环模式选项
      watchSlidesProgress: true,
      watchSlidesVisibility: true,
      slidesPerView: 3,
      //自动播放
      autoplay: {
        delay: 6000,
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
  },
  methods: {
    /** 前往联系我们页面 */
    loopImg(index) {
      new Swiper(".customer-swiper", {
        loop: true, // 循环模式选项
        slidesPerView: index,
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
    },
    GoTop(num, num2) {
      window.scrollTo(0, num);
    },
    goLink(link) {
      if (link) {
        window.open(link)
      }
    }
  },
  watch: {
    '$route': function () {
      const { hash } = this.$route
      if (hash) {
        const index = hash.indexOf('#')
        const str = hash.slice(1, Infinity)
        const id = document.getElementById(str)
        if (index !== -1 && id) {
          this.GoTop(id.offsetTop, id.clientHeight)
        }
      }
    }
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
  height: 900px;
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

/*  2*/
#swiper2 {
  height: 600px;
}
#swiper2 .banner-swiper {
  width: 100%;
  height: 100%;
}
#swiper2 .banner-swiper .swiper-slide img {
  width: 100%;
  height: 100%;
}
#swiper2 .banner-swiper .swiper-slide{
  position: relative;
}
#swiper2 .banner-swiper .swiper-slide-title {
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
#swiper2 .banner-swiper .swiper-slide-title > h1{
  font-size: 50px;
  margin-top: 12%;
}
#swiper2 .banner-swiper .swiper-slide-title > p{
  font-size: 20px;
  margin-top: 1%;
  font-weight: 700;
}

/* 大数据管理系统 */
#bigData {
  padding: 100px;
  transition: all ease 0.6s;
  box-sizing: border-box;
}
#bigData .bigData-title {
  padding-bottom: 10px;
  border-bottom: 1px solid #ccc;
  text-align: center;
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
  color: #333;
  height: 400px;
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

.swiperFlex {
  display: flex;
  align-items: center;
  width: 300px;
  height: auto;
}

.swiper-yellow {
  color: yellow;
}

.swiper-abs {
  position: absolute;
  left: 5%;
  top: 5%;
  color: #fff;
  font-size: 16px;
  font-weight: bold;
  z-index: 10;
}

.swiper-ul {
  list-style: disc;
}

.swiper-ul li {
  font-size: 24px;
}

.swiper-slide-h3{
  font-size: 45px;
  margin-top: 15%;
  line-height: 60px;
  font-weight: bold;
}
.swiper-slide-h3Xs {
  margin-top: 20%;
}
.swiper-p {
  margin: 0;
  padding: 0;
  font-weight: 100!important;
  line-height: 30px!important;
}
.customer-logo2 img {
  width: 200px;
  height: 200px;
}

.clients {
  display: flex;
  box-sizing: border-box;
  padding: 30px 0;
  justify-content: center;
  flex-wrap: wrap;
}
.clients ul {
  display: flex;
  align-items: center;
}
.clients ul li {
  text-align: center;
  padding: 0 20px;
  position: relative;
}
.clients ul li span {
  display: block;
}
.blue {
  color: #66afe9;
  font-weight: bold;
}
.line {
  height: 100%;
  background: #66afe9;
  width: 1%;
  position: absolute;
  right: 0;
  top: 0;
}
.swiper-title-p {
  line-height: 40px;
  font-size: 50px!important;
}
.swiper-content-p2 {
  line-height: 45px;
  font-size: 30px;
}
/* 媒体查询（手机） */
@media screen and (max-width: 768px) {
  .swiper-img {
    width: 1000px!important;
    transform: translateX(-25%);
    height: 100%;
  }
  .customer-content1 {
    padding: 0!important;
    border: none!important;
  }
  .customer-content2 {
    padding: 0!important;
  }
  .swiper-p {
    margin: 0;
    padding: 0;
    font-weight: 100!important;
    line-height: 20px!important;
    font-size: 16px!important;
  }
  .swiper-content-p2 {
    line-height: 30px;
    font-size: 16px;
  }
  .swiper-title-p {
    font-size: 20px!important;
    line-height: 50px;
  }
  .swiper-slide-h3{
    font-size: 25px;
    margin-top: 40%;
    line-height: 40px;
    font-weight: bold;
  }
  .swiper-ul li {
    font-size: 14px;
  }
  #swiper {
    height: 500px;
  }
  #bigData {
    padding: 30px;
  }
  #bigData .bigData-title {
    font-size: 20px;
    text-align: center;
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
    width: 48px;
    height: 48px;
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
  .mediaLogo {
    border-radius: 10px;
  }
  .mediaLogo img{
    width: 50px!important;
    height: 50px!important;
    border-radius: 10px;
  }
  .swiper-width {
    width: 150px!important;
    border-radius: 20px;
    border: 1px solid #f5f5f5;
    margin: 0 10px;
    height: 200px;
  }
  .clients ul li {
    padding: 0 5px;
  }
  .swiper-slide-h3Xs {
    margin-top: 40%;
    font-size: 26px;
  }
  .customer-block {
    padding: 0!important;
  }
  .customer-content2-p {
    margin: 0;
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

.fontWhite {
  color: #ffffff!important;
}

.swiper-content-button a {
  margin: 0 10px;
}

</style>


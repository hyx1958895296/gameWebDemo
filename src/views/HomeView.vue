<template>
  <div class="home">
    <div class="header pd_14">
      <div class="login_in_out_area">
        <div></div>
        <div>
          <span>登录</span>
          <span class="sep">|</span>
          <span>注册</span>
        </div>
      </div>
      <div class="search-area">
        <img src="@/assets/17173_logo.png" alt="" class="icon_logo">
        <div class="search">
          <div class="search-top">
            <div class="par-input"><input type="text" class="search-top-left" placeholder="梦幻西游"></div>
            <div class="search-top-right">
              <img src="@/assets/搜索.png" alt="" class="search_icon">
            </div>
          </div>
        </div>
        <div class="search-area-right">
          <img src="@/assets/173app.png" alt="" class="icon-173app">
          <span class="text">一起一起上</span>
        </div>
      </div>
      <div class="search-bottom">
        <div class="search-bottom-null"></div>
        <div>
          <span>黎明之海</span>
          <span>剑网3缘起</span>
          <span>怀旧频道</span>
          <span>开局送赵云</span>
        </div>
      </div>
    </div>
    <div class="recycle">
      <img src="@/assets/b.jpg" alt="">
    </div>
    <div class="main">
      <div class="flex-center">
        <div class="nav-list pd_14 flex-center">
          <div>
            <div class="nav" v-for="(nav, index) in navListLeft" :key="index">{{ nav.title }}</div>
          </div>
          <div class="flex-center nav-right">
            <div class="mr-20 ml-5 nav-right-l">H5小游戏</div>
            <div class="mr-20 ml-5 nav-right-r">
              <div>网页游戏</div>
              <div class="num">25</div>
            </div>
          </div>
        </div>
      </div>
      <div class="under-line"></div>

      <div class="item-list pd_14">
        <div class="nav-item" v-for="(item, index) in navListBottomL" :key="index">{{ item.title }} </div>
        <div class="nav-item" v-for="(itemr, index) in navListBottomR" :key="index">{{ itemr.title }}</div>
        <div>
          <span class="today-test-text">今日测试：</span>
          <span class="num2">5</span>
          <span class="c-orange">款游戏</span>
        </div>
      </div>
      <div class="picture pd_14">
        <div class="picture1"></div>
        <div class="picture2"></div>
      </div>
      <div class="tab pd_14">
        <div class="tab-under-line">
          <div class="tab-game">
            <div class="tab-game-item">
              <div class="hot-spot"></div>
              <div>热门</div>
              <i class="arrow"></i>
            </div>
            <div class="tab-game-item">
              <div class="hot-spot"></div>
              <div>新游</div>
            </div>
            <div class="tab-game-item">
              <div class="hot-spot"></div>
              <div>手游</div>
            </div>
            <div class="tab-game-item">
              <div class="hot-spot"></div>
              <div>页游</div>
            </div>
            <div class="tab-game-item">
              <div class="hot-spot"></div>
              <div>按A-Z</div>
            </div>
          </div>
          <div class="tab-search">
            <div class="search-top">
              <div><input type="text" class="search_inp" placeholder="梦幻西游"></div>
              <div class="tab-search-inp">
                <img src="@/assets/搜索1.png" alt="" class="icon_search">
              </div>
            </div>
          </div>
          <div>
            <img src="@/assets/添加.png" alt="" width="20px" height="20px" style="vertical-align: middle;">
            <span>添加游戏</span>
          </div>
        </div>
        <div class="classic">
          <div class="first-rows">
            <div class="tit">经&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;典</div>
            <div class="tit-name">
              <div v-for="(titItem, index) in tit" :key="index">{{ titItem.name }}</div>
            </div>
          </div>
          <div class="first-rows">
            <div class="tit">爆&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;款</div>
            <div class="tit-name">

              <div style="padding:5px 2px; background-color: #fd5600; color: #fff;">开局召火凤</div>
              <div>流放之路</div>
              <div>传奇3</div>
              <div>失落的方舟</div>
              <div>神佑释放</div>
              <div style="font-size:15px; color: #ff5c00; font-weight: 900;">1.76上班族高爆传奇</div>
              <div>永恒之塔</div>
              <div style="color:#ff5c00">天龙八部荣耀版</div>
              <div>元神</div>
              <div>逆水寒</div>
              <div>最终幻想14</div>

            </div>
          </div>
          <div class="first-rows">
            <div class="tit">玩家好评</div>
            <div class="tit-name">
              <div v-for="(titItem, index) in tit1" :key="index">{{ titItem.title }}</div>
            </div>
          </div>
          <div class="first-rows">
            <div class="tit">晚回青春</div>
            <div class="tit-name">
              <div v-for="(titItem, index) in tit" :key="index">{{ titItem.name }}</div>
            </div>
          </div>
          <div class="first-rows">
            <div class="tit">近期可玩</div>
            <div class="tit-name">
              <div v-for="(titItem, index) in tit2" :key="index">{{ titItem.title }}</div>
            </div>
          </div>
          <div class="first-rows">
            <div class="tit">即将上线</div>
            <div class="tit-name">
              <div v-for="(titItem, index) in tit" :key="index">{{ titItem.name }}</div>
            </div>
          </div>
          <div class="first-rows">
            <div class="tit">手&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;游</div>
            <div class="tit-name">
              <div v-for="(titItem, index) in tit" :key="index">{{ titItem.name }}</div>
            </div>
          </div>
          <div class="first-rows">
            <div class="tit">页&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;游</div>
            <div class="tit-name">
              <div v-for="(titItem, index) in tit" :key="index">{{ titItem.name }}</div>
            </div>
          </div>
        </div>
        <img src="@/assets/lm-0728-1100x120.jpg">
        <div class="main-first">
          <div class="main-first-picture">
            <img src="@/assets/ESKdjYbqjbgsDep.jpg" alt="">
            <div class="hd">
              <h3 class="tit2">
                <div class="tit2">
                  <div class="ico-tit-line"></div>
                  <a href="">游戏视频</a>
                  <img src="@/assets/app2021-ico-phone.png" alt="">
                  <a href="" style="font-size:13px">APP看视频更方便</a>
                </div>
                <div style="font-size:12px">
                  更多视频》
                </div>
              </h3>
            </div>
            <div class="grid-gap">
               <div>
              <img src="@/assets/TEEVD.jpg" alt="">
            </div>
            <div>
              <img src="@/assets/HKYTO.jpg" alt="">
            </div>
            <div>
              <img src="@/assets/mlGYrWb.jpg" alt="">
            </div>
            <div>
              <img src="@/assets/gyYiIPb.jpg" alt="">
            </div>
            </div>
           
          </div>
          <div></div>
          <div>sdafsadf</div>
        </div>
      </div>
    </div>
    <div class="footer">
      <div class="footer-content">
        <div class="footer-first-row">
          <div class="footer-content-first-row">
            <h3 class="tit1">
              <div class="ico-tit-line"></div>
              <a href="">17173最新动态：</a>
            </h3>
            <div class="tit1">·</div>
            <div class="tit1">
              <a href="">17173全程报道2021年ChinaJoy</a>
            </div>
          </div>
          <div class="search">
            <div class="search-top">
              <div class="par-input"><input type="text" class="search-top-left" placeholder="梦幻西游"></div>
              <div class="search-top-right">
                <img src="@/assets/搜索.png" alt="" class="search_icon">
              </div>
            </div>
          </div>
        </div>
        <div class="grid">
          <div class="footer-second-row">
            <p>
              <a href="">关于17173</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">家长监护</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">人才招聘</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">广告服务</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">商务洽谈</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">联系方式</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">客服中心</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">友情链接</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">版权保护投诉指引</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">隐私政策</a>
              <span class="ml-10">|</span>
            </p>
            <p>
              <span>Copyright © 2001-2022 17173. All rights reserved. 北京智汇游信息技术有限公司</span>
              <span class="ml-10">|</span>
              <span class="ml-10">京ICP证140516号</span>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">京ICP备14014454号-1</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">工业和信息化部备案管理系统网址</a>
            </p>
            <p>
              <a href="">京网文[2021]3682-980号</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">互联网出版许可证</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">信息网络传播视听节目许可证</a>
              <span class="ml-10">|</span>
              <img src="@/assets/beian-icon.png" alt="" class="img-style ml-10">
              <a href="">闽公网安备 35010002000107</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">广播电视节目制作经营许可证 (京)字第10528号</a>
            </p>
            <p>
              <span>违法和不良信息举报电话：0591-88500579</span>
              <span class="ml-10">|</span>
              <span class="ml-10">举报邮箱：</span>
              <a href="" class="ml-10">17173jubao@cyou-inc.com</a>
              <span class="ml-10">|</span>
              <a href="" class="ml-10">未成年人专用投诉举报邮箱：</a>
            </p>
            <p>
              <span>健康游戏公告：抵制不良游戏</span>
              <span class="ml-20">拒绝盗版游戏</span>
              <span class="ml-20">注意自我保护</span>
              <span class="ml-20">谨防受骗上当</span>
              <span class="ml-20">适度游戏益脑</span>
              <span class="ml-20">沉迷游戏伤身</span>
              <span class="ml-20">合理安排时间</span>
              <span class="ml-20">享受健康生活</span>
            </p>
            <p>
              <img src="@/assets/logo-f-cert.png">
              <img src="@/assets/logo-f-xin.png" class="ml-10" alt="">
              <img src="@/assets/cert-cyberpolice.png" class="ml-10" alt="">
            </p>
          </div>
          <div class="footer-right">
            <div>
              <img src="@/assets/微信.png" width="36px" height="36px" class="ml-20">
              <div class="triangle"></div>
              <img src="@/assets/app2021-logo-bot.png" class="ml-10">
            </div>
            <img src="@/assets/code-114x114.png" class="ml-20 qr-code" alt="">
            <div class="text">关注17173微信</div>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navListLeft: [
        { title: '资讯中心' },
        { title: '新游戏 · 今日开服' },
        { title: '游戏下载' },
        { title: '发号平台' },
        { title: '有料社区' },
        { title: '17173影视' },
        { title: '17173视频' },
        { title: '新页游 · 开测 · 开服' },
      ],
      navListBottomL: [
        { title: '排行榜' },
        { title: '找游戏' },
        { title: '游戏测评' },
        { title: '新游测试表' },
        { title: '怀旧服测试表' },
        { title: '过审游戏' },
      ],
      navListBottomR: [
        { title: '/' },
        { title: '100%拿周边' },
        { title: '/' },
        { title: '有偿试玩' },
        { title: '/' },
        { title: '鉴赏家' },
        { title: '/' },
        { title: '次世代' },
        { title: '/' },
        { title: '元宇宙' },
        { title: '/' },
        { title: '更多?' },
      ],
      tit: [
        { name: '地下城与勇士' },
        { name: '800%超爆单职业' },
        { name: '魔兽世界' },
        { name: '梦幻西游' },
        { name: '魔域' },
        { name: '奇迹MU' },
        { name: '剑灵' },
        { name: '热血江湖' },
        { name: '笑傲江湖高清服' },
        { name: '剑网3' },
        { name: '英雄联盟' },
        { name: '新天龙八部' },
      ],
      tit1: [
        { title: "暗黑·永恒不朽" },
        { title: "镇魂街·天生为王" },
        { title: "梦幻新诛仙" },
        { title: "宝可梦大集结" },
        { title: "剑网3缘起" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
      ],
      tit2: [
        { title: "暗黑·永恒不朽" },
        { title: "镇魂街·天生为王" },
        { title: "梦幻新诛仙" },
        { title: "宝可梦大集结" },
        { title: "剑网3缘起" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "剑网3缘起" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "剑网3缘起" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
        { title: "暗黑·永恒不朽" },
      ]
    }
  },
}
</script>
<style>
.home {
  width: 1536px;
  margin: 0 auto;
  padding: 0;
  min-width: 1380px;
  box-sizing: border-box;
}

.pd_14 {
  padding: 0 14%;
}

.ml-10 {
  margin-left: 10px;
}

.ml-20 {
  margin-left: 20px;
}

.login_in_out_area {
  display: flex;
  justify-content: space-between;
  align-items: center;
  line-height: 30px;
  font-size: 12px;
}

.sep {
  margin: 0 0.7em;
  color: #ccc;
}

.icon_logo {
  background-color: white;
}

.search-area {
  display: flex;
  justify-content: space-between;
  padding: 0 1%;
  align-items: center;
}

.search-top {
  display: flex;
}

.search-bottom span {
  margin-top: 3px;
  font-size: 12px;
  margin-right: 10px;
}

.search-bottom {
  display: flex;
  justify-content: center;
  margin-bottom: 5px;
}

.search-bottom-null {
  margin-right: 8px;
}

.search-top-left {
  width: 348px;
  height: 36px;
  font-size: 14px;
  line-height: 36px;
  outline: none;
  text-indent: 0.7em;
  border: 1px solid rgb(255, 205, 0);
}

.search_inp {
  width: 180px;
  height: 22px;
  font-size: 12px;
  outline: none;
  text-indent: 0.7em;
  border-radius: 30px 0 0 30px;
  border: 1px solid #ececec;
  border-right: none;
}

.par-input input::placeholder {
  color: #cccecb;
}

.search_icon {
  width: 32px;
  height: 32px;
  text-align: center;
  margin-top: 4.5px;
}

.search-top-right {
  text-align: center;
  width: 60px;
  height: 40px;
  background-color: rgb(255, 205, 0);
}

.search-area-right .text {
  font-size: 12px;
  color: rgb(122, 122, 122);
}

.search-top-right:hover {
  background-color: rgb(255, 228, 0);
}

.icon-173app {
  width: 35px;
  height: 35px;
  margin-right: 7px;
  vertical-align: middle;
}

.search-area-right {
  cursor: pointer;
}

.recycle {
  position: absolute;
  z-index: 1000;
  top: 50px;
  width: 20px;
  height: 80px;
  cursor: pointer;
}

.under-line {
  border-bottom: 3px solid #f3cb2e;
  padding: 0;
}

.nav-list {
  height: 40px;
  line-height: 40px;
  width: 100%;
}

.nav {
  float: left;
  margin-right: 25px;
  font-size: 16px;
  line-height: 40px;
  text-decoration: none;
  color: #3b4745;
  cursor: pointer;
  position: relative;
}

.list {
  margin-left: 20px;
}

.nav::before {
  content: '';
  position: absolute;
  left: 50%;
  bottom: 0;
  width: 100%;
  top: 28px;
  height: 2px;
  background-color: #fc2f70;
  transform-origin: center;
  transform: translate(-50%, 0) scaleX(0);
  transition: transform 0.3s ease-in-out;
}

.nav:hover {
  color: #fc2f70;
  text-decoration: red;
}

.nav:hover::before {
  transform: translate(-50%, 0) scaleX(1);
}

.num {
  position: absolute;
  top: 3px;
  left: 56px;
  width: 20px;
  font: bold 12px/12px SimSun, sans-serif;
  color: #fff;
  text-align: center;
  background-color: #ff5c00;
  border-radius: 6px 6px 6px 0;
}

.nav-right {
  color: #666;
  font-size: 14px;
  cursor: pointer;
}

.nav-right-r {
  position: relative;
}

.nav-right-l:hover {
  text-decoration: underline;
}

.nav-right-r:hover {
  text-decoration: underline;
}

.item {
  float: left;
  margin-right: 25px;
  font-size: 14px;
  line-height: 40px;
  text-decoration: none;
  color: #3b4745;
  cursor: pointer;
}

.item:hover {
  text-decoration: underline;
}

.item-list {
  height: 40px;
  line-height: 40px;
  font-size: 14px;
}

.nav-item {
  display: flex;
  float: left;
  margin-right: 16px;
  color: #666;
}

.nav-item:hover {
  text-decoration: underline;
}

.today-test-text {
  color: #999;
  font-size: 14px;
}

.num2 {
  display: inline-block;
  border: 1px solid #ff5c00;
  color: #ff5c00;
  height: 16px;
  line-height: 19px;
  padding: 0px 3px;
  border-radius: 2px;
  margin-right: 7px;
  font-size: 12px;
}

.num2:hover {
  background-color: #ff5c00;
  color: white;
}

.icon_search {
  width: 15px;
  height: 15px;
  vertical-align: middle;
}

.c-orange {
  color: #ff5c00;
  font-size: 14px;
}

.picture {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.picture1 {
  width: 100%;
  height: 80px;
  background-image: url(@/assets/xx-0726-54780.jpg);
  background-repeat: no-repeat;
}

.picture2 {
  width: 98%;
  height: 80px;
  background-image: url(@/assets/tlbb-0705-547x80.jpg);
  background-repeat: no-repeat;
}

.hot {
  position: absolute;
  left: 30px;
}

.tab-game {
  width: 470px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.tab-under-line {
  display: grid;
  grid-template-columns: 6fr 1.5fr 1fr;
  height: 30px;
  align-items: center;
  border-bottom: 1px solid #f3cb2e;
}

.hot-spot {
  width: 12px;
  height: 15px;
  background-image: url(@/assets/b1.png);
  background-position: -49px -74px;
  margin: 0px 5px 3px 0px;
}

.arrow {
  width: 8px;
  height: 5px;
  font-size: 0;
  line-height: 0;
  background: url(@/assets/b1.png) no-repeat 0 -110px;
  position: absolute;
  left: 17%;
  bottom: -4px;
  margin-left: -4px;
}

.tab-game-item {
  display: flex;
  align-items: center;
}

.tab {
  padding-top: 11px;
  position: relative;
  height: 27px;
}

.search-inp {
  width: 100px;
  outline: none;
  border-radius: 30px;
  text-indent: 0.5em;
}

.tab-search-inp {
  width: 24px;
  height: 24px;
  border: 1px solid #ececec;
  border-left: none;
  border-radius: 0px 30px 30px 0px;
}

.classic {
  padding: 7px 1%;
}

.first-rows {
  display: flex;
  margin: 3px 0;
}

.tit {
  margin-right: 18px;
  font-weight: 900;
  color: #0069b9;
  font-size: 12px;
  width: 52px;
}

.tit-name {
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-size: 12px;
  width: 100%;
}

.flex-center {
  display: flex;
  justify-content: space-between;
}

.mr-20 {
  margin-right: 20px;
}

.ml-5 {
  margin-left: 5px;
}

.footer {
  background-color: rgb(51, 51, 51);
  padding: 20px 14% 35px 14%;
  margin-top: 40px;
  position: relative;
  top: 1100px;
  /* position: fixed; */
  /* bottom: 1px; */
}

.ico-tit-line {
  width: 3px;
  height: 14px;
  background: #ffcd00;
  margin-right: 10px;
}

.tit1 {
  display: flex;
  align-items: center;
  color: #fff;
}

.tit1 a {
  color: #fff;
  text-decoration: none;
  font-size: 16px;

}

.tit2 {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.tit2 a {
  text-decoration: none;
  font-size: 16px;

}

.grid-gap{
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 15px;
}

.main-first {
  padding: 20px 0;
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
}

.main-first-picture {
  margin-right: 20px;
}


.footer-content-first-row {
  display: flex;
}

.footer-first-row {
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 2px solid #3f3f3f;
  height: 42px;
}

.footer-second-row {
  font-size: 12px;
}

.footer-second-row a {
  color: #8c8984;
  text-decoration: none;
}

.footer-second-row span {
  color: #8c8984;
}

.img-style {
  vertical-align: middle;
  margin-right: 5px;
}

.grid {
  display: grid;
  grid-template-columns: 5fr 1fr;
  align-items: center;
}

.triangle {
  width: 0;
  height: 0;
  font-size: 0;
  border: 6px dashed transparent;
  border-bottom-style: solid;
  border-bottom-color: #fff;
  position: absolute;
  left: 20%;
  margin-left: -6px;
  top: 35px;
}

.footer-right {
  position: relative;
}

.qr-code {
  display: block;
  position: relative;
  top: 7px;
  border: 2px solid #fff;
}

.text {
  padding: 10px 0px;
  font-size: 12px;
  color: #999;
  margin-top: 8px;
  padding-left: 37px;
}
</style>

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
    <div class="main">
      <div class="flex-center">
        <div class="nav-list pd_14 flex-center">
          <div>
            <div class="nav" v-for="(nav, index) in navListLeft" :key="index">{{ nav.title }}</div>
          </div>
          <div class="flex-center nav-right">
            <div class="mr-20 ml-5">H5小游戏</div>
            <div class="mr-20 ml-5 position-rla">
              <div>网页游戏</div>
              <div class="num">25</div>
            </div>
          </div>
        </div>
      </div>
      <div class="under-line"></div>
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
  padding: 0 14.5%;
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
  font-size: 14px;
  text-indent: 0.7em;
  border: 1px solid rgb(255, 205, 0);
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
  left: 63px;
  width: 20px;
  font: bold 12px/12px SimSun, sans-serif;
  color: #fff;
  text-align: center;
  background-color: #ff5c00;
  border-radius: 6px 6px 6px 0;
}

.position-rla{
  position: relative;
}

.nav-right{
  color: #666;
  font-size: 14px;
  cursor: pointer;
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
</style>

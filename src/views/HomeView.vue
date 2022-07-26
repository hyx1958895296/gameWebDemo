<template>
  <div class="home">
    <div class="header">
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
  </div>
</template>

<script>
export default {

}
</script>
<style>
.home {
  margin: 0 auto;
  padding: 0 14.5%;
  min-width: 1170px;
  box-sizing: border-box;
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
}

.search-bottom-null{
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
.par-input input::placeholder{color:  #cccecb;} 

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
</style>

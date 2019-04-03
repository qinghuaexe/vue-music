<template>
  <div class="Home">
    <div class="fixed">
      <header class="header">
        <div class="title">
          <img class="icon" src="../../assets/imgs/icon_logo.png">
          网易云音乐
        </div>
      </header>
      <div class="tabs">
        <router-link class="tab" tag="div" to="/home/recommend">
          <div>推荐音乐</div>
        </router-link>
        <router-link class="tab" tag="div" to="/home/hotsearch">
          <div>热歌榜</div>
        </router-link>
        <router-link class="tab" tag="div" to="/home/search">
          <div>搜索</div>
        </router-link>
      </div>
    </div>
    <div class="content">
      <router-view></router-view>
    </div>
  </div>
</template>
<script>
export default {}
</script>
<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.Home {
  .fixed {
    top: 0;
    left: 0;
    right: 0;
    background: #fff;
    position: fixed;
    z-index: 9999;
  }
  .header {
    height: 60px;
    background: #f72400;
    display: flex;
    align-items: center;
    .title {
      margin-left: 10px;
      margin-right: 10px;
      font-size: 22px;
      color: #fff;
      display: flex;
      align-items: center;
      .icon {
        margin-right: 4px;
        width: 35px;
        height: 35px;
      }
    }
  }
  .tabs {
    display: flex;
    border-bottom: 1px solid #ddd;
    .tab {
      width: 33.33333333%;
      height: 40px;
      line-height: 40px;
      display: flex;
      align-items: center;
      justify-content: center;
      > div {
        padding: 0 4px;
      }
    }
    & .router-link-active {
      > div {
        border-bottom: 2px solid #f72400;
      }
    }
  }
  .content {
    padding-top: 100px;
    height: 1000px;
  }
}
</style>


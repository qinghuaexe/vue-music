<template>
  <div class="Recommend">
    <div class="musicList">
      <div>推荐歌单</div>
    </div>
    <div class="wrapper">
      <div class="item" v-for="i in 6" :key="i">
        <div class="picture">
          <div class="iconwrapper">
            <div class="iconEar"></div>344.4万
          </div>
          <img
            src="http://p1.music.126.net/eHAwwM3gm7SImiWzYK2rBQ==/109951163718244781.webp?imageView&thumbnail=370x0&quality=75&tostatic=0&type=webp"
          >
        </div>
        <div class="itemInfo">这首歌真甜 有和我一起酸的嘛</div>
      </div>
    </div>
    <div class="newSong">
      <div>最新音乐</div>
    </div>
    <div class="songWrapper">
      <div class="song" v-for="i in 6" :key="i">
        <div class="songLeft">Show Me Love
          <div class="singer">
            <img src>
            singer,singer,singer
          </div>
        </div>
        <div class="songRinght">
          <img src>
        </div>
      </div>
    </div>
    <footer>
      <div>
        <img class="iconWangyi" src="../../../assets/imgs/icon_logo.png">
        网易云音乐
      </div>
    </footer>
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
.Recommend {
  .musicList {
    padding: 10px 0;
    font-size: 16px;
    > div {
      height: 18px;
      padding-left: 6px;
      border-left: 2px solid #f72400;
    }
  }
  .wrapper {
    padding-top: 10px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    .item:nth-child(n + 4) {
      margin-top: 16px;
    }
    .itemInfo {
      margin: 0px 5px;
    }
    .item {
      font-size: 14px;
      width: 32.888888%;
      .picture {
        font-size: 12px;
        position: relative;
        > img {
          width: 136px;
          height: 136px;
        }
      }
      .iconwrapper {
        top: 0px;
        right: 0px;
        position: absolute;
        display: flex;
        justify-content: center;
        align-items: center;
        .iconEar {
          width: 10px;
          height: 10px;
          background: green;
        }
      }
    }
  }
}
.newSong {
  padding: 16px 0;
  > div {
    height: 18px;
    padding-left: 6px;
    border-left: 2px solid #f72400;
  }
}
.songWrapper {
  .song {
    padding: 5px 5px;
    display: flex;
    justify-content: center;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid #ddd;
    .songLeft {
      font-size: 17px;
      color: #333;
      width: 85%;
      .singer {
        font-size: 12px;
        display: flex;
        align-items: center;
        > img {
          width: 8px;
          height: 8px;
          background: green;
        }
      }
    }
    .songRinght {
      width: 15%;
      display: flex;
      justify-content: center;
      align-items: center;
      > img {
        background: green;
        width: 20px;
        height: 20px;
      }
    }
  }
}
footer {
    margin-top:40px;
  > div {
      font-size: 40px;
      display: flex;
    align-items: center;
    justify-content: center;
    .iconWangyi {
      width: 45px;
      height: 45px;
    }
  }
}
</style>

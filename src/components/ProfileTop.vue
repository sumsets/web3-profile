<template>
  <div id="head">
    <div id="upper-head" :style="{ backgroundImage: 'url(' + imageUrl + ')' }">
      <div id="status-bar">
        <span id="status-bar-left">
          09:41
        </span>

        <div id="status-bar-right">
          <img class="right-bar-icons" src="@/assets/MobileSignal.svg" alt="sinyal" />

          <profile-top-wifi class="right-bar-icons" :degree="wifiLevel"></profile-top-wifi>

          <img class="right-bar-icons" src="@/assets/Battery.svg" alt="bateri ikonu" />
        </div>
      </div>

      <div id="back-more-bar">
        <img src="@/assets/Frame.svg" alt="back" />
        <img src="@/assets/Group 65.svg" alt="more" />
      </div>

      <div id="wallet-token-bar">
        <div id="wallet">
          <img  id="wallet-icon" src="@/assets/wallet-icon.svg" alt="wallet-icon">
          <span id="director">{{code}}</span>
        </div>

        <div id="token">
          <img id="token-icon" src="@/assets/tokens.svg" alt="tokens" />
          <span id="token-total">{{token}}</span>
        </div>
      </div>
    </div>

    <div id="upper-head2" :style="{ backgroundImage: 'url(' + imageUrl2 + ')' }">
      <div id="profile-section">
        <img :src="pp" alt="">

        <div id="user-id">
          {{user}}
        </div>

        <div id="badges">
          <img :src="badge1" alt="">
          <img :src="badge2" alt="">
          <img :src="badge3" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProfileTopWifi from './ProfileTopWifi.vue';

export default {
  components: {
    ProfileTopWifi,
  },
  data() {
    return {
      mobil: 'sinyal',
      wifiLevel: 3,
      back: '../assets/Frame.svg',
      more: '././assets/Group 65.svg',
      code: 'Ox134...5bed',
      token: '420',
      pp: './assets/unsplash_6anudmplLw4.svg',
      user: 'Leroy Watson',
      badge1: './assets/Ranking 1.svg',
      badge2: './assets/Fast Graduate.svg',
      badge3: './assets/Top Student.svg',
      // eslint-disable-next-line
      imageUrl: require('@/assets/top-background.svg'),
      // eslint-disable-next-line
      imageUrl2: require('@/assets/top2-background.svg'),
    };
  },
};
</script>

<style scoped lang="scss">
#head {
  background-color: #E5E5E5;
}
#upper-head {
  height: 154px;
  position: relative;
  z-index: 1;
}
#status-bar {
    color: white;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 13px 24px;
}
#status-bar-right{
    display: flex;
    flex-wrap: wrap;
    }

.right-bar-icons {
  padding-left:5px;
}

#back-more-bar{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 10px 24px;
}
#wallet-token-bar{
    display: flex;
    justify-content: space-between;
    padding: 8px 3px;
    align-items: center;
    margin-top: 20px;

}
#wallet{
    display: flex;
    border: 1px solid #BBD5DE;
    border-radius: 8px;
    background-color: #BBD5DE;
    padding: 4px 9px;
    margin-left: 15px;
    align-items: center;
}
#wallet-icon{
    padding-right: 5px;
}
#director {
 text-decoration: underline;
 font-size: 12px;
}
#token{
    display: flex;
    margin-right: 15px;
    align-items: center;
}
#token-total{
 font-size: 20px;
}
#profile-section{
    height: 158px;
    justify-content: space-between;
    margin-top: -50px;
    display: flex;
    flex-direction: column;
    align-items: center;
}
</style>

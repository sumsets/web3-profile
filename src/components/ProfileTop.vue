<template>
<div id="head">
  <div id="status-bar">
    <span id="status-bar-left">
      09:41
    </span>

    <div id="status-bar-right">
      <!-- <img src="@/assets/mobil.png" /> -->

      <profile-top-wifi :degree="wifiLevel"></profile-top-wifi>

      <!-- <img src="@/assets/battery.png" alt="bateri ikonu" /> -->
    </div>
  </div>

    <div id="back-more-bar">
    <div id="back-button">{{back}}</div>
    <div id="more-button">{{more}}</div>
    </div>
    <div id="wallet-token-bar">
    <div id="wallet">
    <div id="wallet-icon">{{dolar}}</div>
    <div id="director">{{name}}</div>
    </div>
    <div id="token">
    <div id="token-icon">{{euro}}</div>
    <div id="token-total">{{token}}</div>
    </div>
    </div>
    <div id="profile-section">
    <img :src="pp" alt="">
    <div id="user-id">{{user}}</div>
    <div id="badges">
    <img :src="badge1" alt="">
    <img :src="badge2" alt="">
    <img :src="badge3" alt="">
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
      wifiLevel: 1,
      back: '../assets/Frame.svg',
      more: '././assets/Group 65.svg',
      dolar: '$',
      euro: '€',
      name: 'Metehan',
      token: '1001',
      pp: './assets/unsplash_6anudmplLw4.svg',
      user: 'Leroy Watson',
      badge1: './assets/Ranking 1.svg',
      badge2: './assets/Fast Graduate.svg',
      badge3: './assets/Top Student.svg',
    };
  },
};
</script>

<style scoped lang="scss">
#status-bar {
    color: rgb(5, 5, 8);
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 15px 24px;
}
#status-bar-right{
    display: flex;
    flex-wrap: wrap;
    }
#back-more-bar{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 15px 24px;
}
#wallet-token-bar{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 15px 3px;
}
#wallet{
    display: flex;
    flex-wrap: wrap;
}
#token{
    display: flex;
    flex-wrap: wrap;
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

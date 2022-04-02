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
        <img src="@/assets/chain.svg" alt="more" />
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

    <div id="lower-head" :style="{ backgroundImage: 'url(' + imageUrl2 + ')' }">
      <div id="profile-section">
        <img id="pp" src="@/assets/pp.svg" alt="avatar" />

        <span id="user-name">
          {{user}}
        </span>

        <div id="badges">
          <img class="badge" src="@/assets/badge-fast.svg" alt="more" />
          <img class="badge" src="@/assets/badge-student.svg" alt="more" />
          <img class="badge" src="@/assets/badge-ranking-1.svg" alt="more" />
        </div>
      </div>
    </div>

    <div id="description-block">
      <p id="description-text">
        {{description}}
      </p>
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
      wifiLevel: 3,
      code: 'Ox134...5bed',
      token: '420',
      user: 'Leroy Watson',
      description: 'I am an experienced content writer and digital marketing expert, with a proven track record of writing engaging...',
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
  background-color: #F7F7FA;
}
#upper-head {
  position: relative;
  z-index: 1;
  padding-bottom: 5px;
}
#status-bar {
  color: white;
  display: flex;
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
#lower-head {
  margin-top: -55px;
  padding-bottom: 72px;
}
#profile-section{
  justify-content: space-between;
  display: flex;
  flex-direction: column;
  align-items: center;
}
#pp {
  z-index: 1;

}
#user-name {
  color:#333333;
  font-size: 22px;
  padding: 10px;
}
.badge {
  margin: 0px 4px;
}
#description-block {
  display: flex;
  justify-content: center;
  margin-top: -60px;
}
#description-text {
  color:#333333;
  font-size: 16px;
  line-height: 24px;
  width: 300px;
  border-radius: 8px;
  padding: 20px 17px;
  background-color: #FFFFFF;
  margin: 0;
}
</style>

<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <h1>Activity History</h1>
      </div>
    </div>
    <div class="menu">
      <img src="../assets/calendarz.png" alt="" />
      <div class="activity">
        <h2>Last Activity: Friday</h2>
        <img src="../assets/activ.png" alt="">
      </div>
    </div>
    <div class="main">
      <div class="inf">
        <router-link to="/Info">
          <img src="../assets/info.png" alt="" />
        </router-link>
      </div>
      <div class="home">
        <router-link to="/LoggedIn">
          <img src="../assets/home.png" alt="" />
        </router-link>
      </div>
      <div class="profile">
        <router-link to="/Profile">
          <img src="../assets/profile.png" alt="" />
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "loginComp",
  props: {},
};
</script>

<style scoped lang="scss">
.activity {
    margin: 0 auto;
  h2 {
    text-align: center;
    width: 100%;
    margin-top: 1em;
  }

  img {
    width: 80%;
    margin-left: 4.5em !important;
  }
}

.main {
  bottom: 0;
  position: fixed;
  display: flex;
  background-color: #8ec6c5;
  width: 100%;
  height: 4em;
  border-radius: 20px 20px 0 0;

  .inf {
    flex-grow: 1;
    text-align: center;
    margin-top: 1em;
  }

  .home {
    flex-grow: 1;
    text-align: center;
    margin-top: 1em;
  }

  .profile {
    flex-grow: 1;
    text-align: center;
    margin-top: 1em;
  }
}

.header {
  display: flex;
  width: 100%;
  background-color: #8ec6c5;
  height: 6em;
  border-radius: 0px 0px 20px 20px;

  .left {
    flex-grow: 1;

    h1 {
      color: white;
      text-align: center;
      line-height: 3em;
    }
  }
}

.menu {
  display: flex;
  flex-wrap: wrap;

  img {
    margin: 0 auto;
    margin-top: 2em;
    border-radius: 3px;
  }
}
</style>

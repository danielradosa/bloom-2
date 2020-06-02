<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <h1>Avaible Tools</h1>
      </div>
    </div>
    <div class="menu">
      <router-link to="/Mood">
      <div class="journal">
        <div class="left-text">
          <h3>Mood Journal</h3>
        </div>
        <div class="right-icon">
          <img src="../assets/book.png" alt="" />
        </div>
      </div>
      </router-link>
      <router-link to="/Goals">
        <div class="goals">
          <div class="left-text">
            <h3>Daily Goals</h3>
          </div>
          <div class="right-icon">
            <img src="../assets/user.png" alt="" />
          </div>
        </div>
      </router-link>
      <router-link to="/History">
      <div class="history">
        <div class="left-text">
          <h3>Activity History</h3>
        </div>
        <div class="right-icon">
          <img src="../assets/calendar.png" alt="" />
        </div>
      </div>
      </router-link>
    </div>
    <div class="main">
      <div class="inf">
        <router-link to="/Info">
          <img src="../assets/info.png" alt="" />
        </router-link>
      </div>
      <div class="home">
        <img src="../assets/active-home.png" alt="" />
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
.flower {
  margin-left: -4.2em;
  margin-top: -2em;
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
  z-index: 2;

  img {
    margin-top: 1em;
    margin-left: 1em;
  }

  a {
    margin: 0 auto;
    text-decoration: none;
  }

  .history {
    display: flex;
    width: 18em;
    background-color: #6983aa;
    padding: 1em;
    height: 6em;
    margin: 0 auto;
    margin-top: 2em;
    border-radius: 20px;
    color: white;
    box-shadow: 3px 6px 10px rgba($color: #000000, $alpha: .18);

    .left-text {
      flex-grow: 1;
      margin-left: 1em;
      line-height: 4em;
    }

    .right-icon {
      flex-grow: 1;
      margin-left: 1em;
    }
  }

  .goals {
    display: flex;
    width: 18em;
    background-color: #8ec6c5;
    padding: 1em;
    height: 6em;
    margin: 0 auto;
    margin-top: 2em;
    border-radius: 20px;
    color: white;
    box-shadow: 3px 6px 10px rgba($color: #000000, $alpha: .18);

    .left-text {
      flex-grow: 1;
      margin-left: 1em;
      line-height: 4em;
    }

    .right-icon {
      flex-grow: 1;
      margin-left: 1em;
    }
  }

  .journal {
    display: flex;
    width: 18em;
    background-color: #8566aa;
    padding: 1em;
    height: 6em;
    margin: 0 auto;
    margin-top: 4em;
    border-radius: 20px;
    color: white;
    box-shadow: 3px 6px 10px rgba($color: #000000, $alpha: .18);

    .left-text {
      flex-grow: 1;
      margin-left: 1em;
      line-height: 4em;
    }

    .right-icon {
      flex-grow: 1;
      margin-left: 1em;
    }
  }
}
</style>

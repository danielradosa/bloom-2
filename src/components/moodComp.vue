<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <h1>Mood Tracker</h1>
      </div>
    </div>
    <div class="menu">
      <div class="mood-pick">
        <div class="top">
          <h3>How was your day today?</h3>
        </div>
        <div class="mid">
          <img src="../assets/happy.png" alt="" />
          <img src="../assets/medium.png" alt="" />
          <img src="../assets/sad.png" alt="" />
        </div>
        <div class="slider">
          <input
            type="range"
            min="1"
            max="3"
            value="1"
            class="slider"
            id="myRange"
          />
        </div>
      </div>
    </div>
    <div class="next">
          <router-link to="/Write">
          <button>CONTINUE</button>
          </router-link>
      </div>
      <img src="../assets/flower4.png" width="50%" alt="" class="flower">
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
        <router-link to="/">
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

.slider {
  background-color: #8ec6c5;
  -webkit-appearance: none;
  appearance: none;
  border-radius: 20px;
  width: 100%;
  height: 25px;
  outline: none;
  opacity: 0.9;
  -webkit-transition: 0.2s;
  transition: opacity 0.2s;
}

.slider:hover {
  opacity: 1;
}

.slider::-webkit-slider-thumb {
  -webkit-appearance: none;
  appearance: none;
  width: 25px;
  height: 25px;
  background: white;
  cursor: pointer;
  border-radius: 25px;
}

.slider::-moz-range-thumb {
  width: 25px;
  height: 25px;
  cursor: pointer;
}

.mood-pick {
  display: flex;
  flex-wrap: wrap;
  width: 18em;
  background-color: #8566aa;
  padding: 1em;
  border-radius: 20px;
  height: 12em;
  margin: 0 auto;
  margin-top: 6em;

  .top {
    color: white;
    text-align: center;
    width: 100%;
    margin-top: 1em;
  }

  .mid {
    color: white;
    text-align: center;
    width: 100%;
  }

  .slider {
    color: white;
    text-align: center;
    width: 100%;
  }
}

.next {
    margin-top: 4em;
    text-align: center;

    button {
        text-align: center;
        background-color: #8ec6c5;
        padding: 1em;
        border-radius: 20px;
    }
}

a {
  text-decoration: none;
  color: white;

  .logout {
    background-color: #8ec6c5;
    bottom: 7em;
    margin-left: 2em;
    position: fixed;
    padding: 1em;
    border-radius: 20px;
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
    padding: 1.3em;
  }
}
</style>

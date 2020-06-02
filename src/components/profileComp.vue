<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <h1>Profile</h1>
      </div>
    </div>
    <div class="profi">
        <b>Name:</b> Isabelle Carrot <br>
        <b>Dx:</b> Social Anxiety    <br>
        <b>Age:</b> 21  <br>
        <b>Last active:</b> Now
    </div>
    <img src="../assets/flower3.png" width="30%" alt="" class="flower">
    <div class="menu">
        <router-link to="/">
          <button class="logout">LOG OUT</button>
        </router-link>
        <img src="../assets/girl.png" alt="">
    </div>
    <div class="main">
        <div class="inf">
           <router-link to="/Info"> <img src="../assets/info.png" alt=""> </router-link>
        </div>
        <div class="home">
           <router-link to="/LoggedIn"> <img src="../assets/home.png" alt=""> </router-link>
        </div>
        <div class="profile">
            <img src="../assets/active-profile.png" alt="">
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "loginComp",
  props: {}
};
</script>

<style scoped lang="scss">
.profi {
  display: block;
  margin: 0 auto;
  width: 12em;
  margin-top: 2em;
  font-size: 1.5em;
  color: #8566aa;
}

.flower {
  margin-left: -2em;
  margin-top: 2em;
}

a {
  text-decoration: none;
  color: white;

  .logout {
    background-color: #8566aa;
    bottom: 7em;
    margin-left: 2em;
    position: fixed;
    padding: 1em;
    border-radius: 20px;
    box-shadow: 3px 6px 10px rgba($color: #000000, $alpha: .2);
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
        margin-left: 1em;
        margin: 0 auto;
        bottom: 3.9em;
        position: fixed;
        margin-left: 10em;
    }

    
}

</style>

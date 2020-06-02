<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <h1>Information</h1>
      </div>
    </div>
    <div class="menu">
        <p>Hi and welcome,
          <br>
          <br>
          This app will be your 
          helper in your healing journey
          and if you have any questions
          feel free to contact us on our
          informational website.
          <br>
          <br>
          <a href="https://danielradosa.com/bloom/">INFO WEB</a>
        </p>
    </div>
    <img src="../assets/flower9.png" width="50%" alt="" class="flower">
    <div class="main">
        <div class="inf">
            <img src="../assets/active-info.png" alt="">
        </div>
        <div class="home">
           <router-link to="/LoggedIn"> <img src="../assets/home.png" alt=""> </router-link>
        </div>
        <div class="profile">
           <router-link to="/Profile"> <img src="../assets/profile.png" alt=""> </router-link>
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
.flower {
  margin-left: 10em;
  margin-top: -1.8em;
}

p {
  display: block;
  width: 12em;
  margin: 0 auto;
  margin-top: 2em;
  font-size: 1.5em;
  color: #6983aa;

  a {
  color: white;
  background-color: #6983aa;
  box-shadow: 3px 6px 10px  rgba($color: #000000, $alpha: .18);
  padding: 1em;
  border-radius: 20px;
  font-size: 16px;
  text-decoration: none;
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
        margin-top: 1em;
        margin-left: 1em;
    }

    
}

</style>

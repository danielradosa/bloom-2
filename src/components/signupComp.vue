<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <h1>Sign Up</h1>
      </div>
    </div>
    <div class="form">
      <div class="email">
        <h4>E-Mail</h4>
        <input type="text" />
      </div>
      <div class="invite">
        <h4>Invite Code</h4>
        <input type="text" />
      </div>
      <div class="back">
        <div class="left">
          <router-link to="/"> <button class="buck">Back</button> </router-link>
        </div>
        <div class="right">
          <router-link to="/LoggedIn"> <button>Sign Up</button> </router-link>
        </div>
      </div>
    </div>
    <img class="flower" src="../assets/flower2.png" width="50%" alt="">
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
  margin-left: -3em;
  margin-top: 4.1em;
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

.form {
  display: flex;
  flex-wrap: wrap;

  .email {
    margin: 0 auto;
    margin-top: 4em;

    h4 {
      color: #6983aa;
      margin-left: 1em;
    }

    input[type="text"] {
      background-color: #8ec6c5;
      margin-top: 0.5em;
      height: 3em;
      padding: 1em;
      color: white;
      width: 12em;
      border-radius: 20px;
    }
  }

  .invite {
    margin: 0 auto;
    margin-top: 2em;

    h4 {
      color: #6983aa;
      margin-left: 1em;
    }

    input[type="text"] {
      background-color: #8ec6c5;
      margin-top: 0.5em;
      height: 3em;
      padding: 1em;
      color: white;
      width: 12em;
      border-radius: 20px;
    }
  }
}

input[type="text"]:focus {
  outline-width: 0;
  box-shadow: 3px 6px 10px rgba(0, 0, 0, 0.18);
  transition: 0.3s;
}

button:focus {
  outline-width: 0;
  box-shadow: 3px 6px 10px rgba(0, 0, 0, 0.18);
  transition: 0.3s;
}

.back {
  display: flex;
  margin: 0 auto;

  .left {
    margin-right: 2em;
  }
}

.buck {
  background-color: #8991ff;
}

button {
  background-color: #006eff;
  padding: 0.7em;
  width: 7em;
  margin-top: 4em;
  color: white;
  border-radius: 20px;
  text-transform: uppercase;
}
</style>

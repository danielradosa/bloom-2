<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <h1>Welcome to Bloom</h1>
      </div>
    </div>
    <div class="form">
      <div class="but">
       <router-link to="/LoggedIn"> <button>Log in</button> </router-link>
      </div>
      <div class="or">
        <h3>or</h3>
      </div>
      <div class="buttwo">
         <router-link to="/SignUp"><button>Sign up</button></router-link>
      </div>
    </div>
    <img class="flower" src="../assets/flower2.png" width="50%" alt="">
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

  .buttwo {
    width: 100%;
    text-align: center;
    margin-top: 1.5em;

    button {
      background-color: #8ec6c5;
      padding: .7em;
      width: 9em;
      color: white;
      box-shadow: 3px 6px 10px rgba($color: #000000, $alpha: .2);
      text-transform: uppercase;
      border-radius: 20px;
    }
  }

  .but {
    width: 100%;
    text-align: center;
    margin-top: 12em;

    button {
      
      background-color: #8566aa;
      padding: .7em;
      width: 9em;
      color: white;
      border-radius: 20px;
      box-shadow: 3px 6px 10px rgba($color: #000000, $alpha: .2);
      text-transform: uppercase;
    }
  }

  .or {
    width: 100%;

    h3 {
      text-align: center;
      margin-top: 1em;
    }
  }
}

button:focus {
  outline-width: 0;
  box-shadow: 3px 6px 10px rgba(0, 0, 0, .18);
}
</style>

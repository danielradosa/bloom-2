<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <h1>Daily Goals</h1>
      </div>
    </div>
    <img src="../assets/flower6.png" width="30%" alt="" class="flower">
    <div class="menu">
      <v-card flat class="mx-auto" width="300">
        <v-list shaped flat>
          <v-list-item-group v-model="model" multiple>
            <template v-for="(item, i) in items">
              <v-divider v-if="!item" :key="`divider-${i}`"></v-divider>

              <v-list-item
                v-else
                :key="`item-${i}`"
                :value="item"
                active-class="deep-purple--text text--accent-4"
              >
                <template v-slot:default="{ active, toggle }">
                  <v-list-item-content>
                    <v-list-item-title v-text="item"></v-list-item-title>
                  </v-list-item-content>

                  <v-list-item-action>
                    <v-checkbox
                      :input-value="active"
                      :true-value="item"
                      color="deep-purple accent-4"
                      @click="toggle"
                    ></v-checkbox>
                  </v-list-item-action>
                </template>
              </v-list-item>
            </template>
          </v-list-item-group>
        </v-list>
      </v-card>
    </div>
    <div class="btnz">
      <div class="add">
        <button>Add Item</button>
      </div>
      <div class="reset">
        <button>Reset List</button>
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
  data: () => ({
    items: [
      "Go out",
      "Start conversation",
      "Find new friend",
      "Call an old friend",
      "Write in journal",
    ],
    model: ["Carrots"],
  }),
};
</script>

<style scoped lang="scss">
.flower {
  margin-left: -2.6em;
  margin-top: -1em;
}

.btnz {
    display: flex;
    
    .add {
        flex-grow: 1;
        margin-left: 4em;
        margin-top: 4em;

        button {
            background-color: #8566aa;
            padding: 1em;
            color: white;
            border-radius: 20px;
            box-shadow: 3px 6px 10px rgba($color: #000000, $alpha: .2);
        }
    }

    .reset {
        flex-grow: 1;
        margin-top: 4em;

        button {
            background-color: #6983aa;
            padding: 1em;
            color: white;
            border-radius: 20px;
            box-shadow: 3px 6px 10px rgba($color: #000000, $alpha: .2);
        }
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
  margin-left: 1em;
  margin-top: -3em;
}
</style>

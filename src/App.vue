<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light">
      <router-link v-if="!authenticated" class="navbar-brand" :to="{name: 'home'}"><img src="logo.png" width="250" height="80"></router-link>
      <router-link v-if="authenticated" class="navbar-brand" :to="{name: 'team'}"><img src="logo.png" width="250" height="80"></router-link>
      <router-link v-if="authenticated" class="btn btn-info mr-2" to="/tablica" id="properfont">TABLICA</router-link>
      <router-link v-if="authenticated" class="btn btn-info" to="/team" id="properfont">MOJ TIM</router-link>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>  
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
        </ul>
        <router-link v-if="!authenticated" class="btn btn-outline my-2 my-sm-0 mr-2" to="/login" id="properfont">Prijava</router-link>
        <span v-if="authenticated" id="properfont">
                  {{ myuser }}
                  <a @click="logout" class="btn btn-info my-2 my-sm-0 mr-2" href="#" id="properfont">Odjava</a>
        </span>
        <router-link v-if="!authenticated" class="btn btn-outline my-2 my-sm-0 mr-2" to="/register" id="properfont">Registracija</router-link>
      </div>
    </nav>

    <router-view/>

    <div id="footer" class="text-center mt-5" style="font-family:Cuprum; font-size:20px;">@FantasyHNL - Matej Crkvenac</div>
  </div>
</template>

<style >
  #properfont{
    font-family:Cuprum;
    font-size:30px;
  }
</style>

<script type="text/javascript">
import store from '@/store.js'

export default {
  data () {
    return store;
  },
  methods: {
    logout() {
      firebase.auth().signOut()
    }
  },
  mounted () {
    firebase.auth().onAuthStateChanged(user => {
      if (user) {
        console.log("Korisnik je prijavljen kao " + user.email)
        this.authenticated = true
        db.collection("users")
          .doc(user.email)
          .get()
          .then(doc => {
              if (doc.exists) {
                console.log("Document data:", doc.data());
                this.myuser = doc.data().username;
                this.myteam = doc.data().teamname;
              } else {
                // doc.data() will be undefined in this case
                console.log("No such document!");
              }
          });
        this.userEmail = user.email
        if (this.$route.name !== 'team')
          this.$router.push({name: 'team'}).catch(err => console.log(err))
      }
      else {
        console.log("Korisnik nije prijavljen")
        this.authenticated = false
        if (this.$route.name !== 'home')
          this.$router.push({name: 'home'}).catch(err => console.log(err))
      }
    });
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#navbar {
  margin-bottom: 0;
}
#navbar-brand {
  background-color: white;
  margin-bottom: 0px;
  img {
    position: relative;
  }
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

</style>

<template>
  <div class="jumbotron jumbotron-fluid" style="padding: 0.5em; background-image: url(ademi.jpg); background-repeat:no-repeat; background-size:90%; height: 900px; background-position: 50% 50%">
    <h1 class="display-2" style="font-family:Impact; text-align:left; color:transparent; text-shadow:0 0 4px #ffffff; margin-left: 110px;"><b>BUDI I TI DIO EKIPE</b></h1>
<template>
    <div class="register" style="margin-right:1050px; margin-left:400px; margin-top:50px; height: 420px; background: rgba(30, 30, 50, 0.5); border-radius: 20px;">
        <h1 style="font-family:Impact; color:white; padding-top:10px;">REGISTRACIJA</h1>
        <div class="container" style="font-family:Impact; color:white; margin-top:30px;">
            <div class="row">
                <div class="col-sm"></div>
                    <div class="col-sm">
                        <form @submit.prevent=signup action="Team.vue">
                            <div class="form-group" style="width:250px;">
                            <input v-model="email" type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="EMAIL ADRESA"/>
                            </div>
                            <div class="form-group">
                            <input v-model="username" type="text" class="form-control" id="exampleInputUsername1" placeholder="KORISNIČKO IME"/>
                            </div>
                            <div class="form-group">
                            <input v-model="password" type="password" class="form-control" id="exampleInputPassword1" placeholder="LOZINKA"/></div>
                            <div class="form-group">
                            <input v-model="teamname" type="text" class="form-control" id="exampleInputTeam1" placeholder="NAZIV EKIPE"/>
                            </div>
                            <button type="submit" class="btn btn-primary" style="margin-top:10px;background-color:green;border-radius:25px; font-size:20px; color:black; border: none;">REGISTRIRAJ SE</button>
                            <div>
                            <router-link class="btn btn-primary" to="/#" style="margin-top:15px;background-color:red;border-radius:25px; font-size:18px; color:black; border: none;">ODUSTANI</router-link>
                            </div>
                            </form>
                            </div>
                            <div class="col-sm"></div>
                        </div>
                    </div>
  </div>
</template>
</div>
</template>
<script>
export default {  
    data() {
            return {    
                    email: "",
                    username: "",
                    password: "",
                    teamname: ""
        }
    },
    methods: {
        signup(){
            firebase.auth().createUserWithEmailAndPassword(this.email,this.password).then(() => {
                let id = this.email;
                db.collection("users").doc(id).set({
                    teamname: this.teamname,
                    username: this.username
                })
            })
        }
    }
}
</script>
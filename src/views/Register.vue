<template>
  <div class="jumbotron jumbotron-fluid" id="jumboreg" style="background-image: url(ademi.jpg);">
    <h1 class="display-2" id="naslovreg"><b>BUDI I TI DIO EKIPE</b></h1>
<template>
    <div class="register" id="regreg">
        <h1 id="regnaslovreg">REGISTRACIJA</h1>
        <div class="container" id="ctr1">
            <div class="row">
                <div class="col-sm"></div>
                    <div class="col-sm">
                        <form @submit.prevent=signup action="Team.vue">
                            <div class="form-group" style="width:250px;">
                            <input v-model="email" type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="EMAIL ADRESA"/>
                            </div>
                            <div class="form-group" style="width:250px;">
                            <input v-model="username" type="text" class="form-control" id="exampleInputUsername1" placeholder="KORISNIČKO IME"/>
                            </div>
                            <div class="form-group" style="width:250px;">
                            <input v-model="password" type="password" class="form-control" id="exampleInputPassword1" placeholder="LOZINKA"/></div>
                            <div class="form-group" style="width:250px;">
                            <input v-model="teamname" type="text" class="form-control" id="exampleInputTeam1" placeholder="NAZIV EKIPE"/>
                            </div>
                            <button type="submit" class="btn btn-primary" id="tipkareg1">REGISTRIRAJ SE</button>
                            <div>
                            <router-link class="btn btn-primary" to="/#" id="tipkareg2">ODUSTANI</router-link>
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

<style>
    #jumboreg{
        padding: 0.5em;
        background-repeat:no-repeat;
        background-size:cover;
        height:900px;
        background-position: 50% 50%
    }
    #naslovreg{
        font-family:Impact;
        text-align:left;
        color:transparent;
        text-shadow:0 0 4px #ffffff;
        margin-left: 4%;
    }
    #regreg{
        margin-right:58%;
        margin-left:21%;
        margin-top:50px;
        height: 48%;
        width:22%;
        background: rgba(30, 30, 50, 0.5);
        border-radius: 20px;
    }
    #regnaslovreg{
        font-family:Impact;
        color:white;
        padding-top:10px;
    }
    #ctr1{
        font-family:Impact;
        color:white;
        margin-top:30px;
    }
    #tipkareg1{
        margin-top:10px;
        background-color:green;
        border-radius:25px;
        font-size:20px;
        color:black;
        border: none;
    }
    #tipkareg2{
        margin-top:15px;
        background-color:red;
        border-radius:25px;
        font-size:18px;
        color:black;
        border: none;
    }
</style>

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
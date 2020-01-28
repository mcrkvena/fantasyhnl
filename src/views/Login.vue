<template>
  <div class="jumbotron jumbotron-fluid" id="jumbolog" style="background-image: url(ademi.jpg);">
    <h1 class="display-2" id="naslovlog"><b>BUDI I TI DIO EKIPE</b></h1>
<template>
    <div class="login" id="loglog">
        <h1 id="lognaslovlog">PRIJAVA</h1>
        <div class="container" id="ctr2">
            <div class="row">
                <div class="col-sm"></div>
                    <div class="col-sm">
                        <form @submit.prevent="signin">
                            <div class="form-group" style="width:250px;">
                            <input v-model="email" type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="EMAIL ADRESA"/>
                            </div>
                            <div class="form-group" style="width:250px;">
                            <input v-model="password" type="password" class="form-control" id="exampleInputPassword1" placeholder="LOZINKA"/></div>
                            <button type="submit" class="btn btn-primary" id="tipkalog1">PRIJAVI SE</button>
                            <div>
                            <router-link class="btn btn-primary" to="/#" id="tipkalog2">ODUSTANI</router-link>
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
    #jumbolog{
        padding:0.5em;
        background-repeat:no-repeat;
        background-size:cover;
        height:900px;
        background-position: 50% 50%;
    }
    #naslovlog{
        font-family:Impact;
        text-align:left;
        color:transparent;
        text-shadow:0 0 4px #ffffff;
        margin-left: 4%;
    }
    #loglog{
        margin-right:58%;
        margin-left:21%;
        margin-top:50px;
        height:40%;
        background: rgba(30, 30, 50, 0.5);
        border-radius: 20px;
    }
    #lognaslovlog{
        font-family:Impact;
        color:white;
        padding-top:10px;
    }
    #ctr2{
        font-family:Impact;
        color:white;
        margin-top:30px;
    }
    #tipkalog1{
        margin-top:20px;
        background-color:green;
        border-radius:25px;
        font-size:20px;
        color:black;
        border: none;
    }
    #tipkalog2{
        margin-top:20px;
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
                    password: ""
        }
    },
    methods: {
        signin(){
            firebase.auth().signInWithEmailAndPassword(this.email, this.password).catch(function(error){
                console.log(error)
            });
        }
    }
}
</script>
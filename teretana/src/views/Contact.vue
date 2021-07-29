<template>
  <div class="about">
    <div class="about_top">
      <h1>Contact</h1>
    </div>
    <div class="mail">
      <div class="mail_form">
        <input type="text" placeholder="from" v-model="from"/>
        <input type="text" placeholder="subject" v-model="subject"/>
        <textarea name="" id="" cols="30" rows="10" v-model="message"></textarea>
        <button class="send" @click="send">Posalji</button>
      </div>
    </div>
  </div>
</template>
<script>
// @ is an alias to /src
import axios from "axios";
export default {
  name: "Home",
  data() {
    return {
      from: "",
      subject: "",
      message: "",
      baseURL:'http://226b122.mars1.mars-hosting.com'
    };
  },
  methods: {
    // login() {
    //   axios
    //     .post(this.baseURL + "/api/login", {
    //       username: this.username,
    //       password: this.password,
    //     })
    //     .then((res) => {
    //       // this.setSid(res.data.sid)
    //       //   this.changeAdmin(res.data.admin);
    //       console.log(res.data.msg);
    //       console.log(res.data.user);

    //       if (res.data.msg === "OK") {
    //         localStorage.setItem("sid", res.data.sid);
    //         //uzimanje lev_id-a iz prethodne sesije
    //         localStorage.setItem("lev_id", res.data.lev_id);
    //         //
    //         this.changeLogin(true);
    //         this.changeAdmin(res.data.admin);
    //         this.changeUser(res.data.member);
    //         this.changeUsrId(res.data.user.usr_id);
    //         this.$router.push({ path: "/" });

    //         this.msg = "Uspešno si se ulogovao";
    //       } else {
    //         this.msg = res.data.msg;
    //       }
    //     });
    // },
    send() {
      axios.post(this.baseURL + "/api/mail",{from:this.from , subject:this.subject , message:this.message }).then((res) => {
        
        console.log(res.data.data);
      });
    },
  },
  mounted() {},
};
</script>

<style  scoped>
.about {
  width: 100%;
}
.about_top {
  width: 100%;
  height: 250px;
  background: url("../assets/Slika.jpg");
  background-size: cover;
  padding-top: 230px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;
  /* background-attachment: fixed; */
}
.about_top h1 {
  font-size: 60px;
  color: #ffffff;
  font-weight: 600;
  text-transform: uppercase;
  margin-bottom: 15px;
  font-family: "Oswald", sans-serif;
}
.mail {
  justify-content: center;
  display: flex;
}
.mail_form {
  
  display: flex;
  flex-direction: column;
  width: 40%;
  justify-content: center;
  align-items: center;
}
.send {
  margin-top: 20px;
  width: 200px;
  height: 40px;
}
@media only screen and (max-width: 600px) {
  .about_top {
    background: url("../assets/Slika2.jpg");
    background-position: bottom right;
    background-repeat: no-repeat;
    background-size: cover;
  }
}
</style>
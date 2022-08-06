<template>
  <div class="container">
      <div class="left">
      <figure class="heroLogo">
        <img src="../assets/Frame.svg" alt="dribble Logo">
      </figure>
      <div>
        <h1>Discover the world's top <br>
            Designers & Creatives.
        </h1>
      </div>
      <figure>
        <img src="../assets/girlFloor.svg" alt="image of girl on Floor" class="girlOnFloor">
      </figure>
    </div>
    <div class="right">
      <figure>
        <img src="../assets/Frame.svg" alt="dribble Logo">
      </figure>
      <h1 class="notMemberDesktop">Not a member? <span><router-link to="/signup">Sign up now</router-link></span></h1>
      <h1 class="signIn">Sign in to Dribble</h1>
      <div>
        <figure class="twitterLink">
          <a href="#"><img src="../assets/twitterLogo.svg" alt="twitter link"></a> 
        </figure>
      </div>
      <hr>
      <form>
        <label>Username or Email Address</label>
        <input type="text" placeholder="Enter your username or Email" class="usernameInput">
        <label>Password</label>
        <a href="#"><label class="forgetPassword">Forget Password?</label></a> 
        <input type="password" placeholder="Password" class="passwordInput">
        <button class="signInBtn">Sign In</button>      
      </form>
      <h1 class="notMember">Not a member? <span><a href>Sign up now</a></span></h1>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.container{
  max-width: 1200px;
  width: 100%;
  height: 100vh;
  display: flex;
}

.left{
  display: flex;
  flex-direction: column;
  gap: 31px;
  background: #F1CDD7;
  padding-top: 64px; 
  width: 100%;
  max-width: 514px;
}

.girlOnFloor{
  display: none;
}

.heroLogo{
  width: calc(100% - 128px);
  margin: 0 auto;
}

.left h1{
  font-style: normal;
  font-weight: 900;
  font-size: 25px;
  line-height: 30px;
  color: #865C6C;
  width: calc(100% - 128px);
  margin: 0 auto;
}

.right{
  padding-top: 30px;
}

.right img{
  display: none;
}

.notMemberDesktop{
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 20px;
  /* identical to box height, or 143% */
  text-align: right;
  color: #000000;
  margin-bottom: 181px;
}

.signIn{
  font-style: normal;
  font-weight: 900;
  font-size: 24px;
  line-height: 29px;
  /* identical to box height, or 121% */
  color: #0D0C22;
  width: calc(100% - 135px);
  margin: 0 auto;
}

hr{
  width: calc(100% - 135px);
  margin: 39px auto;
}

form{
  width: calc(100% - 135px);
  margin: 0 auto;
}

label{
  font-style: normal;
  font-weight: 900;
  font-size: 15px;
  line-height: 24px;
}

input{
  height: 40px;
  width: 100%;
  margin: 4px 0;
}

input:focus{
  outline: none;
}

input[type=text]{
  padding-left: 10px; 
}

input[type=text]:focus {
  border: 3px solid #EA4C89;
}

input[type=password]{
  padding-left: 10px; 
}

input[type=password]:focus {
  border: 3px solid #EA4C89;
}

.usernameInput{
  background: #FFFFFF;
  border: 1px solid rgba(234, 76, 137, 0.4);
  box-shadow: 0px 0px 0px rgba(234, 76, 137, 0.1);
  border-radius: 8px;
}

.passwordInput{
  background: #FFFFFF;
  border: 1px solid rgba(234, 76, 137, 0.4);
  box-shadow: 0px 0px 0px rgba(234, 76, 137, 0.1);
  border-radius: 8px;
}

::placeholder{
  padding-left: 0px;
}

.password{
  display: flex;
  justify-content: space-between;
  margin: 26px 0px 4px 0px;
}

a{
  text-decoration: none;
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 14px;
  color: #4F3CC9;
}

.signInBtn{
  margin: 22px 0px;
  background: #EA4C89;
  border-radius: 8px;
  height: 40px;
  width: 200px;
  text-align: center;
  border: none;
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 20px;
  color: #fff;
}

.notMember{
  display: none;
}

.forgetPassword{
  float: right;
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 14px;
  /* identical to box height, or 100% */
  color: #4F3CC9;
  margin-top: 4px;
}

@media only screen and (max-width: 860px) {  
.left{
  display: none;
}

.right{
  display: flex;
  flex-direction: column;
  width: calc(100% - 250px);
  margin: 0 auto;
  padding-top: 48px;
}

.signIn{
  margin: 31px 0px 26px 0px
}

.twitterLink{
  padding: 13px 16px;
  background: #F2F2F2;
  border-radius: 8px;
  max-width: 37px;
  text-align: center;
  align-items: center;
  float: right;
}

.signInBtn{
  width: 100%;
}

.notMember{
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 20px;
  /* identical to box height, or 143% */
  text-align: center;
  color: #000000;
}

.notMemberDesktop{
  display: none;
}
}


@media only screen and (max-width: 460px) {  
.left{
  display: none;
}

.right{
  display: flex;
  flex-direction: column;
  width: calc(100% - 40px);
  margin: 0 auto;
  padding-top: 48px;
}

.signIn{
  margin: 31px 0px 26px 0px
}

.twitterLink{
  padding: 13px 16px;
  background: #F2F2F2;
  border-radius: 8px;
  max-width: 37px;
  text-align: center;
  align-items: center;
  float: right;
}

.signInBtn{
  width: 100%;
}

.notMember{
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 20px;
  /* identical to box height, or 143% */
  text-align: center;
  color: #000000;
}

.notMemberDesktop{
  display: none;
}
}

</style>
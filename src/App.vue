<template>
  <div id="app">
    <div class="leftside">
      <h3>
        Million Dollar
      </h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum libero quasi aut voluptatibus error, deserunt repellendus asperiores voluptas temporibus quos? </p>
      
    </div>
    <div class="rightside">
      <h4>VENDOR SIGNUPS </h4>
      <br>
      <input type="text" placeholder="FullName">
      <br>
      <input type="text" placeholder="Bussiness Name">
      <br>
      <input type="text" placeholder="Address">
      <br>
      <input type="text" placeholder="License No">
      <br>
      <input type="email" placeholder="Email">
      <br>
      <input type="text" placeholder="Password">
      <br>
      <span>Remember Me </span>
        <span2> Forgot Password</span2> <br><br>
        <button> SIGNUP</button>
        <br><br>
        <span3>OR</span3>
        <br><br>
        <span4> Already Have An Account?Login</span4>

      
      


    </div>
    <router-view />
  </div>
</template>
<script>
export default {};
</script>
<style>
#app {

  width: 100vw;
  height: 100vh;
  
  display: grid;

  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr ;
  
  
  
}
.leftside{
  place-self: center ;
 
}
.leftside h3 p{
  margin:40% 0 0 10% ;
}

.rightside{
  place-self: right;
  margin-left: 15%;
  margin-top: 18%;
}
input{
  border-radius: 5px;
  width: 40%;
  margin-bottom: 1%;
  background-color:#eee ;
  padding: 9px;
  border: none;
}
h4{
  margin-left: 50px;
}
span{
  font-size: 12px;
  font-weight: 5;
  cursor: pointer;
}
span2{
  font-size: 12px;
  font-weight: 5;
  margin-left: 90px;
  cursor: pointer;
}
button{
  width: 43%;
  padding: 5px;
  border-radius:5px ;
  background-color:blue ;
}
span3{
  margin-left:20% ;
}

span4{
  margin-left:3% ;
  cursor: pointer;
}
h3{
  font-size: 40px;
}
</style>

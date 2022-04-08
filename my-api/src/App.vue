<template>
  <div id="app">
    <h1>Informtion About Users </h1>
       <ul class="style" v-for="item in list" :key="item.id" >
         <li> {{item.id}}  </li>
          <li> {{item.email}}  </li>
           <li> {{item.first_name}}  </li>
            <li> <img :src="item.avatar">  </li>
       </ul>
  </div>
  <router-view/>
</template>

<script>  
import axios from 'axios';
export default{
  data(){
  return{
     list:[]

  };
  },
 async mounted(){
  let result = await axios.get("https://reqres.in/api/users?page=1");
  console.warn("api data",result.data.data);
  this.list=result.data.data;
  },
};
</script>

<style>

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  font-family: 'montserrat',sans-serif;
}

#app{
  
}

.style{
  display: flex;
}
.style li{
  display: inline-block;
  width: 200;
  padding: 30px  50px;
  text-align: center;
  border: 1px solid green;
}


</style>

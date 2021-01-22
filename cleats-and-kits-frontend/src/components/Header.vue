<template>
  <div class="Header">
    <h1>Cleats & Kits</h1>
     
      <div class="topnav">
      <router-link to="/">Kits</router-link>
      <router-link to="#">Shoes </router-link>
       <router-link to="#">Accesories </router-link>
      <router-link to="#">Login</router-link>
      <button class="sign-up"><i class="fas fa-shopping-cart"></i>&nbsp; &nbsp; My Cart</button>
    </div>


  </div>
  
</template>

<style scoped>
h1 {
  padding: 29px;
  text-decoration: line-through green solid 3px;
  font-weight: bolder;
  font-family: Helvetica;
  font-size: 30px;
}

.button {
  position: relative;
  right: 30px;
  top: 30px;
  background-color: transparent;
  outline: none;
}

.sign-up {
  background-color: transparent;
  width: 130px;
  height: 35px; 
  background-color: green;
  color: white;
  font-size: 90%;
  border-color: green;
  outline: none;
  border-radius: 8px;
  box-shadow: none;
  position: absolute;
}

.topnav {
  position: absolute;
  right: 150px;
  color: black;
  letter-spacing: 0px;
  top: 30px;
}

.topnav a {
  float: left;
  color: black;
  text-align: center;
  margin: 2px 30px;
  text-decoration: none;
  font-size: 20px;
}
</style>
<template>
  <nav>
    <input type="checkbox" id="check">
    <label for="check" class="checkbtn">
      <i class="hambuger">&#9776;</i>
    </label>
    <a href="#" class="enlace">
          <img src="https://doctormesarina.com/wp-content/uploads/2018/09/dr-alejandro-mesarina-logo-header-3-300x106.png" alt="" class="logo"/>
    </a>
    <ul>
      <li class="active"><a  href="/">INICIO</a></li>
      <li><a href="profile">Dr. Mesarina</a></li>
      <li><a href="services">Servicios</a></li>
      <li><a href="update">Actualizaciones</a></li>
    </ul>
  </nav>

</template>



<script>
export default {
}
</script>

<style scoped>

nav{
  background: white;
  height: 80px;
  width: 100%;
   z-index:2;
}
.enlace{
  position: absolute;
}
.logo{
  height: 80px;
  margin-left: 10px;
}
nav ul{
  float: right;
  margin-right: 20px;
}
nav ul li{
  display: inline-block;
  line-height: 80px;
  margin: 0 10px;
}
nav ul li a{
  color:black;
  font-size: 18px;
  padding: 7px 13px;
  border-radius: 3px;
  text-transform: uppercase;
  text-decoration: none;
}
li a.active, li a:hover{
  background: #CAE7F7;
  transition: .5s;
}
.checkbtn{
  font-size: 30px;
  color: black;
  float: right;
  line-height: 80px;
  margin-right: 40px;
  cursor:pointer;
  display: none;
}
#check{
  display: none;
}
@media (max-width:952px){
  .enlace{
    padding-left: 20px;
  }
  nav ul li a{
    font-size: 16px;
  }
}
@media(max-width:858px){
  .checkbtn{
    display:block;
  }
  ul{
    position: fixed;
    width:100%;
    height: 100vh;
    background: #EDF9FF;
    top: 80px;
    left: -100%;
    text-align: center;
    transition: all .5s;    
  }
  nav ul li{
    display:block;
    margin: 50px 0;
    line-height: 30px;
  }
  nav ul li a{
    font-size: 20px;
  }
  li a:hover, li a.active{
    background: none;
    color:#2397D7;
  }
  #check:checked ~ul{
    left: 0;
  }
}
</style>

<!--<v-app-bar
      app
      color="white"
      light
  >
    <div class="d-flex align-center">
      <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://doctormesarina.com/wp-content/uploads/2018/09/dr-alejandro-mesarina-logo-header-3-300x106.png"
          transition="scale-transition"
          width="200"
      />

      <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
      />
    </div>

    <v-spacer></v-spacer>

    <div class="hidden-sm-and-down" :value="value">
        <v-btn class="text-toolbar-btn mr-4" to="/" text>Inicio</v-btn>
        <v-btn class="text-toolbar-btn mr-4" to="/profile" text>Dr. Mesarina</v-btn>
        <v-btn class="text-toolbar-btn mr-4" to="/services" text>Servicios</v-btn>
        <v-btn class="text-toolbar-btn mr-4" to="/update" text>Noticias</v-btn>
    </div>
  </v-app-bar>
  -->

  <!--
    
  -->
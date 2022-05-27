<!-- HTML -->
<template>
<div class="PageTop">
  <div class="TopCont">
    <h1 class="heading">Patient Registry</h1>
    <nav>
      <a href="/patient">PATIENT DETAILS</a> 
      <a href="/address">ADDRESS DETAILS</a> 
      <a href="/island">ISLAND DETAILS</a> 
    </nav>
  </div>
</div>
<PatientsForm/>
</template>

<!-- SCRIPT -->
<script>
import PatientsForm from './components/Patients/Patients-NewForm'
// import Islands from './components/Islands-index'
// import Addresses from './components/Addresses-index'

export default {
  components: {
    // Patients,
    // Islands,
    PatientsForm
  },
}

</script>

<!-- STYLE -->
<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
body{
  background-color:#e1e1e1;
}
.PageTop {
  position: fixed;
  top: 0;
  width: 100%;
  height: 140px;
  background-color:#4EA8A8;
 
}
.TopCont{
  position: relative;
  top: 50px;
  max-width: 90%;
  margin:auto;
  display: flex;
  justify-content:space-between;
}
.heading{
  position: relative;
  font-size:30px;
  color:#fff;
}
nav{
  width:500px;
  display: flex;
  justify-content:space-evenly;
  align-items:end;

}
nav a{
  text-decoration: none;
  color: #fff;
  font-weight: bold;
  padding: 10px;
  border-radius: 10px;
}
nav a:hover{
  background-color:#2c3e50;
}

</style>

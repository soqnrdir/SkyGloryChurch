<template>
    <div id="nav">
     <div>
      <h1 style="display:inline-block"  id="sgcText" @click ="clickMainLogo()">하늘영광교회</h1>
      <ul style="display:inline-block" class="navbar-nav">
        <li style="display:inline-block;margin-left:100px;" class="nav-item"><router-link class="nav-link" to="/about">교회소개</router-link></li>
        <li style="display:inline-block;margin-left:100px;" class="nav-item"><router-link class="nav-link" to="/two">설교말씀</router-link></li>
        <li style="display:inline-block;margin-left:100px;" class="nav-item"><router-link class="nav-link" to="/three">교회포토</router-link></li>
        <li style="display:inline-block;margin-left:100px;" class="nav-item"><router-link class="nav-link" to="/four">커뮤니티</router-link></li>
      </ul>
      <p id="sgcSubText" @click ="clickMainLogo()" >Heaven Glory of the Church</p>
      </div>
    </div>
</template>

<script>
export default {
 methods : {
   clickMainLogo() {
     location.href="/";
   }
 }
}
</script>

<style>
#sgcText {
  color :	#00BFFF;
  font-weight: bold;
}

#sgcSubText {
  color :	#4682B4;
  font-weight: bold;
}

#nav {
  height: 120px;
  padding: 30px;
  margin-left:50px;
  margin-right:50px;
  text-align: left;
  background-image: url("../assets/pngegg.png");
  background-repeat : no-repeat;
  background-size : cover;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>

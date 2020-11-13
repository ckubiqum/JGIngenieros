<template>
  <div class="header">
   <div class="container">

   
<div class="hamburger"><img class="menu" src="@/assets/menu.png"></div>
<div class="logo"> <img class="headerLogo" src="@/assets/logo.png"></div>
<div class="account"><img class="user" src="@/assets/user.png"></div>
  


</div>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


p{
    color: aquamarine;
}
.header{
    background-color: #383737;
    width: 100vw;
    height: 50px;
    margin: 0 !important;
    padding: 0px !important;
    position: fixed;
    z-index: 3;
}
.container{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 10px !important;
}
.headerLogo{
    width:auto;
    height: 28px;
}

.menu{
    width:auto;
    height: 28px;
    left: 0px;
}
.user{
    width:auto;
    height: 28px;
    left: 0px;
}
</style>

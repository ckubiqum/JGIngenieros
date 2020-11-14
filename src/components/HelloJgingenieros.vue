<template>
  <div class="roomReservation">

   <div class="dateTimeFilter">
  <h3>RESERVA DE SALAS</h3>
<div class="date">
  <label>Elegir fecha y hora</label>
 <input type="datetime-local" id="meeting-time"
       name="meeting-time" value="AAAA-MM-DDT19:30">
</div>

  
 <div class="filter">
   <label for="dropdown">Filterar</label>
<select id="dropdown">
  <option value="all">Show All</option>
  <option value="todas">Todas las salas</option>
  <option value="libres">Salas libres</option>
  <option value="ocupadas">Salas ocupadas</option>
</select>
<div id="results"></div>
 </div>
 </div>


<div class="hours">

<p class="hour">8am</p>
<p class="hour2">&nbsp;</p>
<p class="hour">10am</p>
<p class="hour2">&nbsp;</p>
<p class="hour">12am</p>
<p class="hour">&nbsp;</p>
<p class="hour">2pm</p>
<p class="hour">&nbsp;</p>
<p class="hour">4pm</p>
<p class="hour">&nbsp;</p>
<p class="hour">6pm</p>
<p class="hour">&nbsp;</p>
<p class="hour">8pm</p>
      </div>


 <div class="backgroundScheme">
   <p class="result"><b>4</b> salas encontradas</p>
    <div class="schemeColumns">

      <div class="columns">
        <div>
  <p class="singleroom">Room 1</p>
  <button class="heart1-red" style="font-size: 30px;">
  <i class="fa fa-heart"></i>
</button>
  </div>
      <div class="schemecolumn">
</div>
<div class="persons">
<img class="user" src="@/assets/user.png" alt="">
      <p>max 10</p></div>
<img class="info" src="@/assets/icon-info.svg" alt="">
      </div>


       <div class="columns">
        <div>
  <p class="singleroom">Room 2</p>
  <button class="heart2-red" style="font-size: 30px;">
  <i class="fa fa-heart"></i>
</button>
  </div>
      <div class="schemecolumn">
</div>
<div class="persons">
<img class="user" src="@/assets/user.png" alt="">
      <p> max 5</p></div>
<img class="info" src="@/assets/icon-info.svg" alt="">
      </div>


      <div class="columns">
        <div>
  <p class="singleroom">Room 3</p>
  <button class="heart3-red" style="font-size: 30px;">
  <i class="fa fa-heart"></i>
</button>
  </div>
      <div class="schemecolumn">
</div>
<div class="persons">
<img class="user" src="@/assets/user.png" alt="">
      <p>max 12</p></div>
<img class="info" src="@/assets/icon-info.svg" alt="">
      </div>


       <div class="columns">
        <div>
  <p class="singleroom">Room 4</p>
  <button class="heart4-red" style="font-size: 30px;">
  <i class="fa fa-heart"></i>
</button>
  </div>
      <div class="schemecolumn">
        </div>
        
        <div class="persons">
<img class="user" src="@/assets/user.png" alt="">
      <p>max 8</p></div>

<img class="info" src="@/assets/icon-info.svg" alt="">
      </div>
      
     </div>
     
    </div>  
   

<div class="ocupation" >

  <div class="freeroom">  
    <span> Reservar sala</span>
</div>

 <div class="ocupiedroom">  
    <span><img class="info" src="@/assets/ocupied.svg" alt=""></span>
</div>

 <div class="freeroom2">  
    <span> Reservar sala</span>
</div>

 <div class="ocupiedroom2">  
    <span><img class="info" src="@/assets/ocupied.svg" alt=""></span>
</div>
</div>

<div class="indicators">
  <hr class="start">
  <hr class="end">
</div>


  </div>


</template>

<script>
export default {
  name: "HelloJgingenieros",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
    font-size: 30px;
    font-weight: 400;
    color: #383737;
    padding-top: 20px;
    margin-bottom: 20px;
}


p{
    font-size: 14px;
    font-weight: 600;
    color: #ffffff;
    position: relative;
    top: 10px;
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: inline-block;
    margin: 0 10px;
}
a {
    color: #42b983;
}


/*  DATE TIME & FILTER */

  .dateTimeFilter{
    width: 75vw;
    height: 240px;
    margin-left: auto;
    margin-right: auto;
    position: relative;
    top: 60px;
}
.filter{
    text-align: left;
}

#meeting-time{
    position: relative;
    font-size: 18px;
    font-family: montserrat;
    font-weight: 500;
    border: solid 0.8px #383737;
    border-left: 0px;
    border-right: 0px;
    border-top: 0px;
    height: 50px;
    text-transform: uppercase;
    letter-spacing: 3px;
    padding: 0px;
    width: 100%;
    margin-bottom: 20px;
    background-color: transparent;
    outline:none;
}

#dropdown{
    width: 100%;
    font-size: 18px;
    font-family: montserrat;
    font-weight: 500;
    border: solid 0.8px #383737;
    border-left: 0px;
    border-right: 0px;
    border-top: 0px;
    height: 50px;
    letter-spacing: 3px;
    background-color: transparent;
    outline:none;
}



.date{
    text-align: left;
}
label{
    color:#383737;
    position: relative;
}

/* ROOM COLUMNS */
.backgroundScheme{
    background-color: #383737;
    width: 100vw;
    height: 935px;
    position: absolute;
    top: 317px;
}
.schemeColumns{
 display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 80%;
    height: 780px;
    position: absolute;
    top: 69px;
    left: 50px;
    float: right;
    z-index: 2; 
    margin: 5px;
}
.schemecolumn{
    width: 20vw;
    max-width: 100px;
    background-color: #ffffff4b;
    border-radius: 4px;
    z-index: 2;
    height: 623px;
    position: relative;
    top: 40px;
}
.columns{
    display: flex;
    flex-direction: column;
    position: relative;
    width: auto;
    margin-left: auto;
    top: -50px;
    justify-content: center;
    text-align: center;
    margin: 0px 1px;
}

.rooms{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 80vw;
  position: relative;
  margin-left: auto;
  margin-right: 22px;
  float: right;
}
.room{
  width: 88px;
  margin: 20px;
}

/* HOURS INDICATOR */
.hours{
  display: flex;
  flex-direction: column;
  line-height: 50px;
  width: 100%;
  z-index: 1;
  margin-left: 10px;
  position: relative;
  top: 210px;

  
}
.hour, .hour2{
  display: flex;
  font-size: 15px;
  font-weight: 600;
  color: #ffffff;
  line-height: 6;
}

.hour2:after, .hour:after{
  content: "";
  flex: 1 1;
  border-bottom: 1px solid #ffffff69;
  margin: auto;
}

/* FAVOURITE INDICATORS */
.heart1-red, .heart2-red, .heart3-red, .heart4-red {
  cursor: pointer;
  position: relative;
  top: 25px;
  text-align: center;
  color: #ffffff;
  background-color: transparent;
  border: none;
  outline:none;
}

.heart1-red:hover, .heart2-red:hover, .heart3-red:hover, .heart4-red:hover {
  color: red;
  background-color: transparent;
  border: none;
  outline:none;
}
.heart1-red:focus, .heart2-red:focus, .heart3-red:focus, .heart4-red:focus{
  color: red;
  background-color: transparent;
  border: none;
  outline:none;
}
.heart-red:active{
  color: red;
  background-color: transparent;
  border: none;
  outline:none;
}

/* INFO BUTTON */
.info{
  position: relative;
  top: 100px;
}

/* PERSONS THAT FIT IN THE ROOM */
.persons{
  display: flex;
  flex-direction: row;
  vertical-align: middle;
  position: relative;
  top: 58px;
  margin-left: auto;
  margin-right: auto;
}
.user{
  position: relative;
  width: 15px;
  height: auto;
  top: 9px;
  margin-right: 10px;
}


/* OCUPATION */
.ocupation{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 80%;
  height: 624px;
  position: absolute;
  top: 468px;
  left: 55px;
  float: right;
  z-index: 2;
}
.freeroom{
  width: 20vw;
  max-width: 100px;
  background: linear-gradient(0deg, #08FFAA 0%, #00EAFD 100%);
  border-radius: 0px;
  z-index: 2;
  height: 90px;
  position: relative;
  top: 174px;
  margin: 0px 1px;


    
}
.freeroom span{
  position: relative;
  font-weight: 600;
  top: 25%;
  text-decoration: underline;
}

.ocupiedroom{
  width: 20vw;
  max-width: 100px;
  background: linear-gradient(0deg, #FF0000 0%, #FF058C 100%);
  border-radius: 0px;
  z-index: 2;
  height: 135px;
  position: relative;
  top: 129px;
}
.freeroom span:hover{
  opacity: 50%;
}
.ocupiedroom span{
  position: relative;
  font-weight: 600;
  top: -33%;
}

.freeroom2{
  width: 20vw;
  max-width: 100px;
  background: linear-gradient(0deg, #08FFAA 0%, #00EAFD 100%);
  border-radius: 0px;
  z-index: 2;
  height: 90px;
  position: relative;
  top: 174px;
  margin: 0px 1px;   
}
.freeroom2 span{
  position: relative;
  font-weight: 600;
  top: 25%;
  text-decoration: underline;
}
.freeroom2 span:hover{
  opacity: 50%;
}

.ocupiedroom2{
  width: 20vw;
  max-width: 100px;
  background: linear-gradient(0deg, #FF0000 0%, #FF058C 100%);
  border-radius: 0px;
  z-index: 2;
  height: 90px;
  position: relative;
  top: 129px;
  margin: 0px 1px;
}
.ocupiedroom2 span{
  position: relative;
  font-weight: 600;
  top: -70%;
}


/* INDICATOR LINES */
.start{
  width: 100vw;
  border: solid 1px #00EAFD;
  position: relative;
  top: -236px;
  z-index: 2;
}
.end{
  width: 100vw;
  border: solid 1px #08FFAA;
  position: relative;
  top: -147px;
  z-index: 2;
}
</style>

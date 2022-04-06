<template>
  <header>
      <div class="dc-navbar">
           <img class="logo-small" src="../assets/dc-logo.png" alt="dc-logo-small">
           <ul>
               <li><a href="#">characters</a></li>
               <li><a href="#">comics</a></li>
               <li><a href="#">movies</a></li>
               <li><a href="#">tv</a></li>
               <li><a href="#">games</a></li>
               <li><a href="#">collectibles</a></li>
               <li><a href="#">videos</a></li>
               <li><a href="#">fans</a></li>
               <li><a href="#">news</a></li>
               <li><a href="#">shop</a></li>
           </ul>

      </div>
     
  </header>
</template>

<script>
export default {
name:'HeaderComponent'
}
</script>

<style scope lang="scss">
$list-style:none;
$font-size:0.6rem;
$text-uppercase: uppercase;
$text-bold:700;
$logo-small: 60px;
$text-darkgray: #5b5a5a;
$d-flex:flex;
$f-direction-column:column;
$link-color: #0b7cec; 
$no-decoration:none;

.dc-navbar{
  display:$d-flex;
  align-items: center;
  justify-content: space-between;

  .logo-small{
    width: $logo-small;
    height: $logo-small;
  }
  ul{
    list-style-type: $list-style;
    display: $d-flex;
    justify-content: space-around;
    
  
    li {
      text-transform: $text-uppercase;
      font-size: $font-size;
      font-weight: $text-bold;
      color:$text-darkgray;
      margin: 0 10px;
      a {
        cursor: pointer;
        text-decoration: $no-decoration;
        color: $text-darkgray;
        &:hover{
          color:$link-color;
        }
      }
   
      
}

}


}


  
 

</style>
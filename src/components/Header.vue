<template>
  <header>
      <div class="dc-navbar">
        <!-- logo dc piccolo -->
           <img class="logo-small" src="../assets/dc-logo.png" alt="dc-logo-small">
           <!-- navbar menu -->
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
@import "../variables";

.dc-navbar {
  display: $d-flex;
  justify-content: space-between;
  align-items:center;
  width:$w-80;
  .logo-small {
    width: 60px;
    height: 60px;
  }
  ul {
    display: $d-flex;
    list-style-type: $list-style;
    li {
      font-size: $font-size-6;
      font-weight: $text-bold;
      text-transform: $text-uppercase;
      margin: 0 10px;
      a {
        text-decoration:$no-decoration;
        color:$text-darkgray;
        padding-bottom: 30px;
        &:hover {
          color: $text-azure;
          border-bottom: 5px solid $text-azure;
        }
      }
    }
  }
}


  
 

</style>
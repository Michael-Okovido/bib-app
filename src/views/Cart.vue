<template>
<nav class="navbar fixed-top navbar-expand-lg navbar-dark " style="background-color: #E98428;" >
       
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
 <a class="navbar-brand" href="#" style="color: white;"><b>BiB</b></a>
   
    <div class="collapse navbar-collapse" id="navbarSupportedContent" >
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active ">
           <router-link to="/home" class="nav-link"  style="color: white;">Home </router-link>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#" style="color: white;">About Us</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-expanded="false" style="color: white;">
            Categories
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
            <a class="dropdown-item" href="#">Iyabeji</a>
            <a class="dropdown-item" href="#">Chicken Republic</a>
            <div class="dropdown-divider"></div>
            <a class="dropdown-item" href="#">Chop life</a>
          </div>
        </li>
       
      </ul>
      
      <form class="form-inline my-2 my-lg-0" >
        <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
        
      </form>
      
    </div>
    <div class="btn btn-primary" data-toggle="modal" data-target="#exampleModal" style="background-color: #E98428; border-color: #E98428;"><i class="bi bi-person-circle">Hi Michael</i></div>
      <div > <router-link to="/cart" class="btn btn-primary" type="button" style="background-color: #E98428 ;border-color: #E98428;"><i class="bi bi-cart3" >Cart</i></router-link></div>
  </nav>
<router-view/>

    <div class="card" style="width: 18rem; margin: auto; margin-top: 50px;">
      <div class="shadow-lg p-3 mb-5 bg-white rounded">
        <img src="../assets/iyabeji.jpeg" class="card-img-top" alt="...">
        <div class="card-body">
          <h5 class="card-title">Iyabeji</h5>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
        <ul class="list-group list-group-flush">
          <li class="list-group-item">White rice(₦) <br> <input type="number" name="" id=""></li>
          <li class="list-group-item">Fried plantain(₦) <br> <input type="number" name="" id=""></li> 
          <li class="list-group-item">Salad(₦) <br> <input type="number" name="" id=""></li>
        </ul>
        <div class="card-body">
          <a href="food1.html" class="btn btn-primary" style="background-color: #EF2936; border-color: #EF2936;">Cancel
          </a>
          <a href="#" type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal" style="background-color: #E98428; border-color: #E98428;">Checkout</a>
        </div>
      </div>
      <!-- Button trigger modal -->
</div>
  
  <!-- Modal -->
  <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">Payment form</h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </button>
        </div>
        <div class="modal-body">
          <h2>Total(₦): 1000</h2>
          <h3>
              ACN: 23478648376 <br>
              BANK: GT BANK <br>
              NAME: OKOVIDO MICHAEL
          </h3>
          <input class="form-control" placeholder="Full name" type="text" name="" id="">
        </div>
        <div class="modal-footer">
        
          <button type="button" class="btn btn-primary" style="background-color: #E98428; border-color: #E98428;">Confirm</button>
        </div>
      </div>
    </div>
  </div>

</template>

<script>


export default {
  
  
}
</script>

<style>
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.7.2/font/bootstrap-icons.css");
</style>

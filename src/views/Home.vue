<template>
 <div class="container-fluid">
       
      
    <nav class="navbar fixed-top navbar-expand-lg navbar-dark " style="background-color: #E98428;" >
       
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
        <a class="navbar-brand" href="#" style="color: white;"><b>BiB</b></a>
       
        <div class="collapse navbar-collapse" id="navbarSupportedContent" >
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item active">
              <router-link to="/home" class="nav-link"  style="color: white;">Home </router-link>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#" style="color: white;">About Us</a>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false" style="color: white;">
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
          
          <form class="d-flex" >
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
            
          </form>
          
        </div>
        <div class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal" style="background-color: #E98428; border-color: #E98428;"><i class="bi bi-person-circle">Hi Michael</i></div>
          <div > <router-link to="/cart" class="btn btn-primary" type="button" style="background-color: #E98428 ;border-color: #E98428;"><i class="bi bi-cart3" >Cart</i></router-link></div>
      </nav>

<router-view/>
      



      <div class="row row-cols-1 row-cols-md-3" style="margin-top: 50px;">
        
        <div class="col mb-4">
          
          <div class="card" style="width: 20rem;">
            <div class="shadow-lg p-3 mb-5 bg-white rounded">
            <img src="../assets/whiterice.jpeg" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">Iyabeji</h5>
              <p class="card-text">White rice and stew.</p>
              <a href="#" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModalCenter" style="background-color: #E98428; border-color: #E98428;">ADD TO CART</a>
            </div>
          </div>
        </div>
      </div>
       
        <div class="col mb-4">

          <div class="card" style="width: 20rem;">
            <div class="shadow-lg p-3 mb-5 bg-white rounded">
            <img src="../assets/friedplantains.jpeg" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">Iyabeji</h5>
              <p class="card-text">Fried plantain</p>
              <a href="#" class="btn btn-primary" style="background-color: #E98428; border-color: #E98428;">ADD TO CART</a>
            </div>
          </div>
        </div>
      </div>
      
        <div class="col mb-4">
            <div class="card" style="width: 20rem;">
              <div class="shadow-lg p-3 mb-5 bg-white rounded">
              <img src="../assets/jollof.jpeg" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card-title">Iyabeji</h5>
                <p class="card-text">Jollof rice</p>
                <a href="#" class="btn btn-primary" style="background-color: #E98428; border-color: #E98428;">ADD TO CART</a>
              </div>
            </div>
          </div>
        </div>
        
          <div class="col mb-4">
            <div class="card" style="width: 20rem;">
              <div class="shadow-lg p-3 mb-5 bg-white rounded">
              <img src="../assets/coleslaw.jpeg" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card-title">Iyabeji</h5>
                <p class="card-text">Salad</p>
                <a href="#" class="btn btn-primary" style="background-color: #E98428; border-color: #E98428;">ADD TO CART</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

     <!-- Modal -->
  <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">Profile</h5>
         
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
         
        </div>
        <div class="modal-body">
          
          <h3>
              NAME: STACY GOBIR <br>
              GENDER: F <br>
              PHONE NO: 090373773783
          </h3>
          
        </div>
        <div class="modal-footer">
        
          <button type="button" class="btn btn-primary" style="background-color: #EF2936; border-color: #EF2936;">Edit</button>
        </div>
      </div>
    </div>
  </div>

  <!-- Modal -->
<div class="modal fade" id="exampleModalCenter" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalCenterTitle"></h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      
      <div class="modal-body">
        <h1>ADDED TO CART!</h1>
      </div>
      <div class="modal-footer">
        
        <a href="cart.html"><button type="button" class="btn btn-primary" style="background-color: #E98428; border-color: #E98428;">Checkout</button></a>
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

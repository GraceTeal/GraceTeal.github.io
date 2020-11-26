# GraceTeal.github.io
<!DOCTYPE html>
<html>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">


<body>
<div class="centered">The Knack Shack</div>
</body>
<style>
 body {
    background-image: url('whitebg.jpg');
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: 100% 100%;
  } 
.centered {
  position: absolute;
  top: 50%;
  left: 25%;
  font-size: 70px;
  font-family: Comfortaa;
}
body {margin:5;}
.navbar {
  overflow: hidden;
  background-color: lightgrey ;
  position: relative;
  top: 5;
  width: 99%;
}
.navbar a {
  float: left;
  display: flex;
  color: #000000;
  text-align: center;
  padding: 7px 20px;
  text-decoration: none;
  font-size: 14px;
}
.navbar a:hover {
  background: black;
  color: white;
}

.logo {
    width:40px;
    position: relative;
    top: 0px;
    right:0px;
  }
  .cart {
    width:40px;
    position: absolute;
    top:13px;
    right:30px;
  }
</style>
<body>
<?php 
session_start();
?>
<div class="navbar">
<?php
if(isset($_SESSION['user_id'])) {?>
  Welcome
  <a href=WebsiteHomePage.php> <img src ="Logo.png" class="logo"/> </a>
  <a href=shoplist.php>Shop</a>
  <a href=logout.php>Logout</a>
  <a href=contact.php>Contact Us</a>
  <a href=shopbasket.php><img src="cart1.png" class="cart"></a>
<?php }
  else { ?>
  <a href=WebsiteHomePage.php> <img src ="Logo.png" class="logo"/> </a>
  <a href=shoplist.php>Shop</a>
  <a href=logIn.php>Login</a>
  <a href=Join.html>Subscribe</a>
  <a href=contact.php>Contact Us</a>
  <a href=shopbasket.php><img src="cart1.png" class="cart"></a>
<?php }
?>
</div>
</body>
<style>
 a {font-family: "Verdana", sans-serif}
body,h1,h2,h3,h4,h5,h6,{font-family: "Verdana", sans-serif;}
</style>
</html>

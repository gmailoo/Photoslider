<!DOCTYPE html>
<html lang="en">
<title>W3.CSS Template</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lato">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
body {
  font-family:Verdana, Geneva, Tahoma, sans-serif}
.mySlides {display: none}
</style>
<body>

<!-- Navbar -->
<div class="w3-top">
  <div class="w3-bar w3-black w3-card">
    <a class="w3-bar-item w3-button w3-padding-large w3-hide-medium w3-hide-large w3-right" href="javascript:void(0)" onclick="myFunction()"></i></a>
    <a href="#" class="w3-bar-item w3-button w3-padding-large">SOME  PICTURES  ARE  SLIDING  MY  ANIMATION</a>
    <a href="javascript:void(0)" class="w3-padding-large w3-hover-red w3-hide-small w3-right"><i class="fa fa-search"></i></a>
  </div>
</div>

<!-- Navbar on small screens (remove the onclick attribute if you want the navbar to always show on top of the content when clicking on the links) -->
<div id="navDemo" class="w3-bar-block w3-black w3-hide w3-hide-large w3-hide-medium w3-top" style="margin-top:92px" width="50%">
  <a href="#SOME PICTURES ARE SLIDING MY ANIMATION" class="w3-bar-item w3-button w3-padding-large" onclick="myFunction()">SOME PICTURES ARE SLIDING MY ANIMATION</a>
</div>

<!-- Page content -->
<div class="w3-content" style="max-width:500px;margin-top:92px" width="50%">

  <!-- Automatic Slideshow Images -->
  <div class="mySlides w3-display-container w3-center">
    <img src="root.jpeg" style="width:95%">
    <div class="w3-display-bottommiddle w3-container w3-text-white w3-padding-32 w3-hide-small">
      <h3></h3>
      <p><b></b></p>   
    </div>
  </div>
  <div class="mySlides w3-display-container w3-center">
    <img src="moon.jpeg" style="width:95%">
    <div class="w3-display-bottommiddle w3-container w3-text-white w3-padding-32 w3-hide-small">
      <h3></h3>
      <p><b></b></p>    
    </div>
  </div>
  <div class="mySlides w3-display-container w3-center">
    <img src="food.jpeg" style="width:95%">
    <div class="w3-display-bottommiddle w3-container w3-text-white w3-padding-32 w3-hide-small">
      <h3></h3>
      <p><b></b></p>    
    </div>
  </div>  
  
<!-- End Page Content -->
</div>

<script>
// Automatic Slideshow - change image every 3 seconds
var myIndex = 0;
carousel();

function carousel() {
  var i;
  var x = document.getElementsByClassName("mySlides");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";  
  }
  myIndex++;
  if (myIndex > x.length) {myIndex = 1}    
  x[myIndex-1].style.display = "block";  
  setTimeout(carousel, 2000);    
}
</script>

</body>
</html>


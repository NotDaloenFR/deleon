<!DOCTYPE html>
<html lang="en">
<title>Introduction to Computing Website</title>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lato">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

  <style>
body {font-family: "Lato", sans-serif}
.mySlides {display: none}
</style>
<body>

<!-- Navbar -->
<div class="w3-top">
  <div class="w3-bar w3-black w3-card">
    <a class="w3-bar-item w3-button w3-padding-large w3-hide-medium w3-hide-large w3-right" href="javascript:void(0)" onclick="myFunction()" title="Toggle Navigation Menu"><i class="fa fa-bars"></i></a>
    <a href="#" class="w3-bar-item w3-button w3-padding-large">HOME</a>
  
   
 <div class="w3-dropdown-hover w3-hide-small">
    <button class="w3-padding-large w3-button" title="More">Conversion <i class="fa fa-caret-down"></i></button>     
    <div class="w3-dropdown-content w3-bar-block w3-card-4">
       <a href="Fahrenheit-to-Celcius.html" class="w3-bar-item w3-button">Fahrenheit to Celcius</a>
       <a href="Metres-to-Feet.html" class="w3-bar-item w3-button">Meters to Feet</a>
    </div>
  </div>

  <div class="w3-dropdown-hover w3-hide-small">
    <button class="w3-padding-large w3-button" title="More">Income Tax Calculator<i class="fa fa-caret-down"></i></button>     
    <div class="w3-dropdown-content w3-bar-block w3-card-4">
       <a href="Income-Tax.html" class="w3-bar-item w3-button">Income Tax calculator online</a>
    </div>
  </div>

  <div class="w3-dropdown-hover w3-hide-small">
    <button class="w3-padding-large w3-button" title="More">Factorial<i class="fa fa-caret-down"></i></button>     
    <div class="w3-dropdown-content w3-bar-block w3-card-4">
      <a href="While-Loop.html" class="w3-bar-item w3-button">While Loop</a>
      <a href="Sum-of-numbers.html" class="w3-bar-item w3-button">Do While Loop</a>
      <a href="Average-of-Numbers.html" class="w3-bar-item w3-button">For Loop</a>
        
   </div>
 </div>

  <div class="w3-dropdown-hover w3-hide-small">
     <button class="w3-padding-large w3-button" title="More">Simple Payroll<i class="fa fa-caret-down"></i></button>     
     <div class="w3-dropdown-content w3-bar-block w3-card-4">
       <a href="Payroll.html" class="w3-bar-item w3-button">Simple Payroll</a>                
     </div>
  </div>

  </div>
</div>

<!-- Navbar on small screens (remove the onclick attribute if you want the navbar to always show on top of the content when clicking on the links) -->
<div id="navDemo" class="w3-bar-block w3-black w3-hide w3-hide-large w3-hide-medium w3-top" style="margin-top:46px">
  <a href="#band" class="w3-bar-item w3-button w3-padding-large" onclick="myFunction()">The Course</a>
</div>

<!-- Page content -->
<div class="w3-content" style="max-width:2000px;margin-top:46px">

   <!-- The Band Section -->
  <div class="w3-container w3-content w3-center w3-padding-64" style="max-width:800px" id="band">
    <h2 class="w3-wide">CS 1130 - Introduction to Computing</h2>
    
   <br>
   <h2>
      Student Assignments:  
      </h2>
      <br>
      <h3>Assignment #1 - Conversion (Celsius to Fahrenheit, Fahrenheit to Celsius, Meters to Feet, Feet to Meters)</h3>
      <h3>Assignment #2 - Income Tax Calculator </h3>
      <h3>Assignment #3 - Factorial (While Loop), Sum (Do While Loop) and Average (For Loop) of First N Natural Numbers</h3>
      <h3>Assignment #4 - Simple Payroll </h3>

   <br>
      <h2>*** All Assignments are Due on December 6, 2023 *** </h2>
      <h4> Upload and launch the pages in your specified github  or w3spaces website. </h4>
     


</div>

   
<!-- End Page Content -->
</div>

<script>
// Automatic Slideshow - change image every 4 seconds
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
  setTimeout(carousel, 4000);    
}

// Used to toggle the menu on small screens when clicking on the menu button
function myFunction() {
  var x = document.getElementById("navDemo");
  if (x.className.indexOf("w3-show") == -1) {
    x.className += " w3-show";
  } else { 
    x.className = x.className.replace(" w3-show", "");
  }
}

// When the user clicks anywhere outside of the modal, close it
var modal = document.getElementById('ticketModal');
window.onclick = function(event) {
  if (event.target == modal) {
    modal.style.display = "none";
  }
}
</script>

</body>
</html>

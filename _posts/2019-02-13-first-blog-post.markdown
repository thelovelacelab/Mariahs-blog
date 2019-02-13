---
title: First Blog post
date: 2019-02-13 02:45:00 Z
---

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />

  </head>
  <style>
    /* CARD CODE */
.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 5);
  
  max-width: 300px;
  margin: auto;
  text-align: center;
  
}

.price {
  color: grey;
  font-size: 22px;
}

.card button {
  border: none;
  outline: 0;
  padding:5px;
  color:#ff5c5c;
  background-color:white;
  text-align: center;
  cursor: pointer;
  width: 100%;
  font-size: 20px;
}

.card button:hover {
  opacity: 0.7;
}

h2 {

  font-family: 'Satisfy', cursive; color:#ff5c5c;
  font-size: 35px;

  
  
}

.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}



.mySlides {display: none;}
img {vertical-align: middle;}

.dot  {
  height: 2px;
  width: 2px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .active2 {
  background-color: #717171;
}

.textstyle {

  word-wrap: break-word;
  width:70%;

  text-align: justify;

}

#more, #more2, #more3, #more4 {
  display: none;
  
  }

.about {

  text-align:justify; 
  /*width:80%; */
  word-wrap: break-word; 
  margin:50px;
  display:in-line-block;
  font-size:18px;
}  

.aboutimage {

  max-width: 100%;
  max-height: 100vh;
  margin:auto;
  padding:0;
  position:relative;

  /* added for title */
  /*float:left;*/
}

p {

  margin:30px;
  text-align:center;

}
    </style>
  
  <body>

 


    <div class="card">
  
    <div id="slideshow1"> 
  <img src="https://imageshack.com/a/img922/1403/JbSZso.png" alt="Dress" style="width:100%" class="mySlides fade">
 
  <img src="https://imageshack.com/a/img923/1144/8NR2Of.png" alt="Dress" style="width:100%" class="mySlides fade">
  
  <img src="https://imageshack.com/a/img923/5162/1W7N1E.png" alt="Dress" style="width:100%" class="mySlides fade">
  </div>
  
  <h2>How to style a  <br> suit 3 different <br> ways</h2>
 
  <p>For this post I have teamed up with Vintage Fair Mall in Modesto CA, to show you guys how I styled this suit from H&M 3 different ways.</p>
  
  <button onclick="myFunction('dots', 'more', 'myBtn')" id="myBtn">Read more</button>
   <span id="dots"> </span>

   <center><p class="textstyle"><span id="more">I got to go on a little shopping spree and I found so many great things at the mall. I got to take over their Instagram stories and show you guys all of my favorite finds. <br>
1. Bring out your inner GIRL BOSS and wear a suit. they are so classy and fun.<br>
2. For a more chic look wear your jacket on your shoulders to give it a little twist.<br>
3. Change up your suit look by only wearing the skirt and adding a fun accessory like I did here with the neck scarf. Adding the scarf in totally changes up the look. <br> 
I desperately tried to try and find other skirt suits but I have not had any luck. Wearing a suit really brings out the #GIRLBOSS in me and it is going to be one of those staple pieces for fall. 
 
I hope you all have a wonderful week ahead and don't let those Monday vibes bring you down.

<br>
<br>
<a href="https://www.macys.com/shop/product/calvin-klein-convertible-danica-sneakers?ID=6362099&CategoryID=17570&cm_kws=191712587757" target="_blank" style="
font-family: 'Poiret One', cursive; font-size:25px"> Sneakers</a>
<br>
<br>
<a href="https://www.stevemadden.com/product/DAISIE/245262.uts" target="_blank" style="
font-family: 'Poiret One', cursive; font-size:25px"> Heels</a>
<br>
<br>
<a href="https://olive-drew.myshopify.com/collections/new-arrivals/products/glen-shirt" target="_blank" style="
font-family: 'Poiret One', cursive; font-size:25px"> T-Shirt</a>

<br>
<br>

<a href="https://www.quayaustralia.com/products/after-hours" target="_blank" style="
font-family: 'Poiret One', cursive; font-size:25px"> Sunnies</a>

<br>
<br>

<a href="https://www2.hm.com/en_us/productpage.0675319002.html" target="_blank" style="
font-family: 'Poiret One', cursive; font-size:25px"> Suit Jacket</a>
<br>
<br>
<br>
</span>
</p>




</center>

</div>
<div style="text-align:center">
  <span class="dot"></span> 
  <span class="dot"></span> 
  <span class="dot"></span> 
</div>

<!-- CARD ENDS -->

   <!-- <script src="script.js">  </script>-->
   <script>

      function myFunction(dots, more, myBtn) {
  var dots = document.getElementById(dots);
  var moreText = document.getElementById(more);
  var btnText = document.getElementById(myBtn);

  if (dots.style.display === "none") {
    dots.style.display = "inline";
    btnText.innerHTML = "Read more"; 
    moreText.style.display = "none";
  } else {
    dots.style.display = "none";
    btnText.innerHTML = "Read less"; 
    moreText.style.display = "inline";
  }
}

// SLIDE SHOW
function showSlides(className, slideStart) {
   var i;
   var myIndex = slideStart;
   var x = document.getElementsByClassName(className);
      for (i = 0; i < x.length; i++) {
        x[i].style.display = "none";
      }
      myIndex++;
      if (myIndex > x.length) {myIndex = 1}

      x[myIndex-1].style.display = "block";

      setTimeout(showSlides, 2000, className, myIndex);
}

showSlides("mySlides", 0);
  
     </script>
  </body>
</html>
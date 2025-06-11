<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Abstract Shape</title>
      <link rel="stylesheet" href="style.css">
  <style>
.grass {
  opacity: 0;
  transition: opacity 0.5s ease, transform 1s ease;
  will-change: opacity, transform;
  
  transform-style: preserve-3d;
 
  width: 100%;
  height: 450px;
  position: absolute;
  opacity: 0;
  transform-origin: bottom center;
  filter:
          drop-shadow(0px -200px 90px rgba(0, 245, 255, 0.3)) 
          drop-shadow(0px -200px 90px rgba(0, 245, 255, 0.3));
}
#grass1 {
  animation: deg 5s 0s infinite ease-in-out forwards,
             move 3s 1.5s linear forwards;
             z-index: -8 !important;
}
#grass2 {
  
  animation: deg 3.8s 0s infinite ease-in-out forwards,
             move 3s 2s linear forwards;
           z-index: -8 !important;
}
#grass3 {
  
  animation: deg 5.6s 0s infinite ease-in-out forwards,
             move 3s 0.7s ease-out forwards;
             z-index: -8 !important;
}
#grass4 {
 
  animation: deg 2.8s 0s infinite ease-in-out forwards,
             move 3s 1s linear forwards;
             z-index: -8 !important;
}
#grass5 {
 
  animation: deg 4.9s 0s infinite ease-in-out forwards,
             move 3s 2.4s linear forwards;
            
  z-index: -8 !important;
}
#grass6 {
 
  animation: deg 3.3s 0s infinite ease-in-out forwards,
             move 3s 3s ease-out forwards;
            
    z-index: -8 !important;
}
@keyframes deg {
  0%{rotate: -3.5deg;}
  50%{rotate: 3deg;}
  100%{rotate: -3.5deg;}
}
@keyframes move {
  0%{transform: scaleY(0);}
  0%{bottom: 16%;}
  100%{bottom: 21%;}
  100%{transform: scaleY(1);}
  100%{opacity: 1;}
}


    /* Shape container */
    #shape-container {
      position: relative;
      width: 330px;
      height: 400px;
      margin: 0px ;
      z-index: 10;
      overflow: visible;
    }


   
body.loading svg {
      display: none;
    }
body{
 padding: 0;
  background: linear-gradient(#020041 20% ,black 70% );
  margin: 0px;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  
}
.appear-move {
  opacity: 0;
  transform: translate(0, 0);
  animation: move 1s 0s both,dg 1s 0s both;
  will-change: opacity, transform;
  
  transform: translateZ(0);
}
svg {
  display: block;
  background: transparent;
  width: 100vw;
  height: 100vh;
  z-index: -9;
}
</style>
</head>

<body class="appear-move" class="loading" >

  
    <!--grass 1-->
    <svg width="300" height="450" viewBox="130 12 30 300" fill="#color" id="grass1" class="grass" >
<defs>
  <linearGradient id="color" x1="0%" y1="20%" x2="0%" y2="50%">
    <stop offset="0%" stop-color="green" />
    <stop offset="100%" stop-color="black" />
  </linearGradient>
</defs>
        <path d="M136 39
             C110 15, 260 120, 180 500 
             C156 250, 195 150, 134 37Z" stroke="transparent" stroke-width="2" fill="url(#color)" transform="translate(-50, 0)"  />
    </svg>
      <!--grass 2-->
    <svg width="300" height="450" viewBox="130 12 30 300" fill="#color" id="grass2" class="grass" >
  <defs>
    <linearGradient id="color" x1="0%" y1="20%" x2="0%" y2="50%">
      <stop offset="0%" stop-color="green" />
      <stop offset="100%" stop-color="black" />
    </linearGradient>
  </defs>
  <g transform="translate(300, 0) scale(-1, 1)">
  <path d="M136 39
             C110 15, 260 120, 180 500 
             C156 250, 195 150, 134 37Z" stroke="transparent" stroke-width="2" fill="url(#color)" transform="translate(-45, 30)"  />
  </g>
    </svg>
     <!--grass 3-->
<svg width="300" height="450" viewBox="120 12 30 300" fill="#color" id="grass3" class="grass">
  <defs>
    <linearGradient id="color" x1="0%" y1="20%" x2="0%" y2="50%">
      <stop offset="0%" stop-color="green" />
      <stop offset="100%" stop-color="black" />
    </linearGradient>
  </defs>
  <path d="M100 90.5
             C110 90, 260 120, 180 520 
             C156 270, 195 150, 100 90" stroke="transparent" stroke-width="1" fill="url(#color)" filter="url(#shadow)" transform="translate(-80, 10)"  >
</svg>
<!--grass 4-->
 <svg width="300" height="700" viewBox="110 80 23 380" fill="#color" id="grass4" class="grass" >
   <defs>
     <linearGradient id="color" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="green" />
      <stop offset="30%" stop-color="green" />
      <stop offset="100%" stop-color="black" />
     </linearGradient>
   </defs>
   <g transform="translate(300, 0) scale(-1, 1)">
   <path d="M123.5 124
             C116 129, 260 140, 180 540 
             C170 270, 190 170, 123 124.5" stroke="transparent" stroke-width="1" fill="url(#color)" filter="url(#shadow)" transform="translate(-40,100)"  >
   </g>
     
 </svg>
 <!--grass 5-->
 <svg width="400" height="450" viewBox="120 50 380 130" fill="#color" id="grass5" class="grass" >
  <defs>
    <linearGradient id="color" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="green" />
      <stop offset="30%" stop-color="green" />
      <stop offset="100%" stop-color="black" />
    </linearGradient>
  </defs>
   <path d="M123.5 200
             C136 205, 260 200, 180 540 
             C170 300, 190 226, 123 200" stroke="transparent" stroke-width="1" fill="url(#color)" filter="url(#shadow)" transform="rotate(-14)" >
 </svg>
 <!--grass 6-->
  <svg width="300" height="450" viewBox="60 50 200 450" fill="#color" id="grass6" class="grass" >
   <defs>
     <linearGradient id="color" x1="0%" y1="20%" x2="0%" y2="100%">
       <stop offset="0%" stop-color="green" />
       <stop offset="100%" stop-color="black" />
     </linearGradient>
   </defs>
   <g transform="translate(300, 0) scale(-1, 1)">
   <path d="M100 280
             C136 245, 260 230, 180 580 
             C170 400, 190 226, 100 280" stroke="transparent" stroke-width="1" fill="url(#color)" filter="url(#shadow)" transform="translate(-75,82)"  >
   </g>
 </svg>
<script>
    window.addEventListener('load', () => {
      document.body.classList.remove('loading');
    });
    
  </script>
</body>

</html>

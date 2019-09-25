<!DOCTYPE html>
<html lang="en">
<head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>Serhat Demirkan Desing @hightlevelMODE</title>
      <meta author="harrnish" content="ig: @harrnish">
      <!-- stylesheet -->
      <link rel="stylesheet" href="style.css">

      <!-- ionicons -->
      <script src="https://unpkg.com/ionicons@4.5.10-0/dist/ionicons.js"></script>

      <!-- jquery -->
      <script src="//cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
     
      <!-- tweenmax - gsap -->
      <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/2.0.2/TweenMax.min.js"></script>
     
</head>
<body>

      <div class="wrapper">
            <div class="hero-section">   
                  <div class="nav">
                        <div class="artist">Gürkan Karataş</div>
                        <div class="watch"><ion-icon name="play"></ion-icon> şimdi izle</div>
                        <div class="menu"><ion-icon name="menu"></ion-icon></div>
                  </div>
                  
                  <div class="hero-gif"></div>

                  <div class="hero-title">
                        <h1 class="glitch" data-text="Underrated">VAY (SEZEN AKSU COVER)</h1>
                        <p>Yeni Cover</p>
                  </div>

                  <div class="rotatethis">
                        <h2 id="rotated">Serhat • Demirkan • Music • Desing • AdManager • </h2>
                  </div>

                  <div class="social-media">
                        <ul>
                              <a href="https://www.youtube.com/channel/UCCG6rkI2kfwcGqmUEWm8Waw"><li>youtube</li></a>
                              <a href="https://www.instagram.com/gurkankrts"><li>instagram</li></a>
                              <a href="https://twitter.com/karasalamander"><li>twitter</li></a>
                        </ul>
                  </div>

                  <div class="listensong">
                        <ul>
                              <audio id="player" src="gurkankaratasvaycover.mp3" audio.play();></audio>
                              <li><ion-icon name="play"onclick="audioHandler()"></ion-icon></li>
                              <li><ion-icon name="musical-notes"></ion-icon></li>
                              <li><ion-icon name="microphone"></ion-icon></li>
                              <li><ion-icon name="videocam"></ion-icon></li>
                              <script>     
                                          var status = false;
                                          var audio = document.getElementById("player");
                                          audio.loop = true;         
                                          audio.play();
                                          function audioHandler(){
                                            if(status == false || audio.paused){
                                              audio.play();
                                              status = true;
                                            }else{
                                              audio.pause();
                                              status = false;
                                            }
                                          }
                              </script>
                        </ul>
                  </div>
            </div>

            <div class="gif-overlay"></div>
      </div>

      <script type="text/javascript" src="https://rawgit.com/peterhry/CircleType/master/dist/circletype.min.js"></script>

<script>
      
      const circleType = new CircleType(document.getElementById('rotated'));   
      TweenMax.from(".artist", 2, {
      delay: 5.4,
      opacity: 0,
      y: 20,
      ease: Expo.easeInOut
      });
      TweenMax.from(".watch", 2, {
      delay: 5.5,
      opacity: 0,
      y: 20,
      ease: Expo.easeInOut
      });
      TweenMax.from(".menu", 2, {
      delay: 5.6,
      opacity: 0,
      y: 20,
      ease: Expo.easeInOut
      });
      TweenMax.from(".rotatethis", 2, {
      delay: 6,
      opacity: 0,
      ease: Expo.easeInOut
      });
      TweenMax.staggerFrom(".social-media ul li", 2, {
      delay: 5.7,
      opacity: 0,
      y: 20,
      ease: Expo.easeInOut
      }, 0.1);
      TweenMax.staggerFrom(".listensong ul li", 2, {
      delay: 5.9,
      opacity: 0,
      y: 20,
      ease: Expo.easeInOut
      }, 0.1);  
      TweenLite.fromTo(".hero-title h1", 0.3, {
            x:-6,
            y:2,
            opacity: 0,
      }, 
      {
            delay: 5,
            x: 6,
            y: -2,
            opacity: 1,
            ease:RoughEase.ease.config({
                  strength:8,
                  points:40, 
                  template:Linear.easeNone, 
                  randomize:false}),
            clearProps:"all"
      });
      TweenLite.fromTo(".hero-title p", 0.3, {
            x:-6,
            y:2,
            opacity: 0,
      }, 
      {
            delay: 9,
            x: 6,
            y: -2,
            opacity: 1,
            ease:RoughEase.ease.config({
                  strength:8,
                  points:40, 
                  template:Linear.easeNone, 
                  randomize:false}),
            clearProps:"all"
      });
</script>
</body>
</html>

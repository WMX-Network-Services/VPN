<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  <title>Update VPN Client</title>
  <style>
*{box-sizing: border-box; -webkit-box-sizing: border-box; }
html, body { height: 100%; }
body { margin: 0; font: 16px/1.3  Verdana, Geneva, Tahoma, sans-serif; }

.CSSgal {
  position: relative;
  overflow: hidden;
  height: 100%; /* Or set a fixed height */
}

.CSSgal .slider {
  height: 100%;
  white-space: nowrap;
  font-size: 0;
  transition: 0.8s;
}

.CSSgal .slider > * {
  font-size: 1rem;
  display: inline-block;
  white-space: normal;
  vertical-align: top;
  height: 100%;
  width: 100%;
  background: none 50% no-repeat;
  background-size: cover;
}

.CSSgal .prevNext {
  position: absolute;
  z-index: 1;
  top: 50%;
  width: 100%;
  height: 0;
}

.CSSgal .prevNext > div+div {
  visibility: hidden; /* Hide all but first P/N container */
}

.CSSgal .prevNext a {
  background: #fff;
  position: absolute;
  width:       60px;
  height:      60px;
  line-height: 60px; /* If you want to place numbers */
  text-align: center;
  opacity: 0.7;
  -webkit-transition: 0.3s;
          transition: 0.3s;
  -webkit-transform: translateY(-50%);
          transform: translateY(-50%);
  left: 0;
}
.CSSgal .prevNext a:hover {
  opacity: 1;
}
.CSSgal .prevNext a+a {
  left: auto;
  right: 0;
}

.CSSgal .bullets {
  position: absolute;
  z-index: 2;
  bottom: 0;
  padding: 10px 0;
  width: 100%;
  text-align: center;
}
.CSSgal .bullets > a {
  display: inline-block;
  width:       30px;
  height:      30px;
  line-height: 30px;
  text-decoration: none;
  text-align: center;
  background: rgba(255, 255, 255, 1);
  -webkit-transition: 0.3s;
          transition: 0.3s;
}
.CSSgal .bullets > a+a {
  background: rgba(255, 255, 255, 0.5); /* Dim all but first */
}
.CSSgal .bullets > a:hover {
  background: rgba(255, 255, 255, 0.7) !important;
}

.CSSgal >s:target ~ .bullets >* {      background: rgba(255, 255, 255, 0.5);}

#s1:target ~ .bullets >*:nth-child(1) {background: rgba(255, 255, 255,   1);}
#s2:target ~ .bullets >*:nth-child(2) {background: rgba(255, 255, 255,   1);}
#s3:target ~ .bullets >*:nth-child(3) {background: rgba(255, 255, 255,   1);}
#s4:target ~ .bullets >*:nth-child(4) {background: rgba(255, 255, 255,   1);}

.CSSgal >s:target ~ .prevNext >* {      visibility: hidden;}

#s1:target ~ .prevNext >*:nth-child(1) {visibility: visible;}
#s2:target ~ .prevNext >*:nth-child(2) {visibility: visible;}
#s3:target ~ .prevNext >*:nth-child(3) {visibility: visible;}
#s4:target ~ .prevNext >*:nth-child(4) {visibility: visible;}

#s1:target ~ .slider {transform: translateX(   0%); -webkit-transform: translateX(   0%);}
#s2:target ~ .slider {transform: translateX(-100%); -webkit-transform: translateX(-100%);}
#s3:target ~ .slider {transform: translateX(-200%); -webkit-transform: translateX(-200%);}
#s4:target ~ .slider {transform: translateX(-300%); -webkit-transform: translateX(-300%);}

.CSSgal{
  color: #fff;  
  text-align: center;
}
.CSSgal .slider h2 {
  margin-top: 10vh;
  font-weight: 200;
  letter-spacing: -0.06em;
  word-spacing: 0.2em;
  font-size: 3em;
}
.CSSgal a {
  border-radius: 50%;
  margin: 0 3px;
  color: rgba(0,0,0,0.8);
  text-decoration: none;
}
</style>
</head>
<body>
<!-- partial:index.partial.html -->
<div class="CSSgal">

  <!-- Don't wrap targets in parent -->
  <s id="s1"></s> 
  <s id="s2"></s>
  <s id="s3"></s>
  <s id="s4"></s>

  <div class="slider">
    <div style="background:#5b8;">
      <h2>Update VPN Client</h2>
      <img src="u.png">
      <p>Responsive Slideshow Gallery created using CSS only<br>by Roko</p>
      <p>Responsive Slideshow Gallery created using CSS only<br>by Roko</p>
      <p>Responsive Slideshow Gallery created using CSS only<br>by Roko</p>
      <p>Responsive Slideshow Gallery created using CSS only<br>by Roko</p>
      <p>Responsive Slideshow Gallery created using CSS only<br>by Roko</p>
    </div>
    <div style="background:#85b;">
      <h2>Slide 2</h2>
    </div>
    <div style="background:#e95;">
      <h2>Slide 3</h2>
    </div>
    <div style="background:#e59;">
      <h2>Slide 4</h2>
    </div>
  </div>
  
  <div class="prevNext">
    <div><a href="#s4"><</a><a href="#s2">></a></div>
    <div><a href="#s1"><</a><a href="#s3">></a></div>
    <div><a href="#s2"><</a><a href="#s4">></a></div>
    <div><a href="#s3"><</a><a href="#s1">></a></div>
  </div>

  <div class="bullets">
    <a href="#s1">1</a>
    <a href="#s2">2</a>
    <a href="#s3">3</a>
    <a href="#s4">4</a>
  </div>

</div>
<!-- partial -->
  
</body>
</html>

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>

* {
  box-sizing: border-box;
}

h1 {
  font-size:20vw;
}
h2 {
  font-size:16vw;
}  
h3 {
  font-size:12vw;
}
h4 {
  font-size:8vw;
}
h5 {
  font-size:4vw;
}
p {
  font-size:2vw;
}   
  
.left {
  background-color: #2196F3;
  padding: 20px;
  float: left;
  width: 20%; /* The width is 20%, by default */
}

.main {
  background-color: #f1f1f1;
  padding: 20px;
  float: left;
  width: 60%; /* The width is 60%, by default */
}

.right {
  background-color: #04AA6D;
  padding: 20px;
  float: left;
  width: 20%; /* The width is 20%, by default */
}

  
  
/* Use a media query to add a break point at 800px: */
@media screen and (max-width: 800px) {
  .left, .main, .right {
    width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
  }
}

</style>
<script src="path/to/script1.js" async></script>
<script src="path/to/script2.js" async></script>  
</head>

<body>

<h2>Media Queries</h2>
<p>Resize the browser window.</p>

<p>Make sure you reach the breakpoint at 800px when resizing this frame.</p>

<div class="left">
  <p>Left Menu</p>
</div>

<div class="main">
  <p>Main Content</p>
</div>

<div class="right">
  <p>Right Content</p>
</div>

<h1 style="font-size:10vw;">Responsive Text</h1>

<p style="font-size:5vw;">Resize the browser window to see how the text size scales.</p>

<p style="font-size:5vw;">Use the "vw" unit when sizing the text. 10vw will set the size to 10% of the viewport width.</p>

<p>Viewport is the browser window size. 1vw = 1% of viewport width. If the viewport is 50cm wide, 1vw is 0.5cm.</p>

<picture>
  <source media="(min-width: 1000px)" srcset="img1.jpg">
  <source media="(min-width: 800px)" srcset="img2.jpg">
  <img src="img3.jpg" style="width:auto;">
</picture>

<div style="text-align:center"> 
  <button onclick="playPause()">Play/Pause</button> 
  <button onclick="makeBig()">Big</button>
  <button onclick="makeSmall()">Small</button>
  <button onclick="makeNormal()">Normal</button>
  <br><br>
  <video id="video1" width="420">
    <source src="sample.mp4" type="video/mp4">
    Your browser does not support HTML video.
  </video>
</div> 

<div>
<p>Count numbers: <output id="result"></output></p>
<button onclick="startWorker()">Start Worker</button> 
<button onclick="stopWorker()">Stop Worker</button>

<p><strong>Note:</strong> Internet Explorer 9 and earlier versions do not support Web Workers.</p>
</div>
  
</body>
</html>

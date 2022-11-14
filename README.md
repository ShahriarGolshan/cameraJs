# cameraJs

### Installation
  
#### Download .zip

[cameraJs.ZIP](https://github.com/ShahriarGolshan/digitalClock/raw/main/DigitalClock.rar)

First we need to add this js file as external references like this

	<script src="/js/camera.js"></script>
  
than we need to create 2 elements a canvas and a video tag

	 <canvas id="canvas" width="320px" height="240px"></canvas>

and 

	 <video id="video" class="box" autoplay></video>
   
than we create a new object of camera

	 const camera = new Camera({
        canvasElement,
        videoElement,
        notSupportingLogic: noSupport
    });
    
than execute init function

	 camera.init();
   
   
 ### create image in canvas
 
you can call this method in eny event you want like onclick and ...

	 camera.createCanvasImage();
   
   
 ### export token image
 
you can export token image from canvas as a blob and uploud or do anything with it

	 const imgBlob = camera.exportImageBlob();;
 
 
 

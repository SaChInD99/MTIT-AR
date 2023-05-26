# MTIT-AR
Augmented Reality




<!DOCTYPE html>
<html>
<head>
    <!-- include A-Frame obviously -->
    <script src="https://aframe.io/releases/0.7.1/aframe.min.js"></script>
    <!-- include ar.js for A-Frame -->
    <script src="https://jeromeetienne.github.io/AR.js/aframe/build/aframe-ar.js"></script>
</head>
<body style='margin : 0px; overflow: hidden;'>
 <a-scene embedded arjs>
    <a-assets>
      <a-asset-item id="tree-obj" src="asst.obj"></a-asset-item> 
    </a-assets>
    <a-marker preset="hiro"> 
       <a-entity obj-model="obj: #tree-obj;" material="src: texture.png " position="0 0 1" rotation="0 10 0" scale="3 3 3"> </a-entity>
    </a-marker>
    <a-entity camera></a-entity>
 </a-scene>
</body>
</html>

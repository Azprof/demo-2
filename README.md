# demo-2
<html>
  <head>
    <script src="//aframe.io/releases/1.5.0/aframe.min.js"></script>
    <script src="https://cdn.jsdelivr.net/gh/MozillaReality/ammo.js@8bbc0ea/builds/ammo.wasm.js"></script>
    <script src="https://cdn.jsdelivr.net/gh/c-frame/aframe-physics-system@v4.2.2/dist/aframe-physics-system.js"></script>
  </head>
  <body>
    <a-scene physics="driver: ammo; debug: true; debugDrawMode: 1;">
      <!-- Camera -->
        <a-entity camera position="0 1.6 5" look-controls wasd-controls></a-entity>
      <!-- Static floor -->
      <a-plane ammo-body="type: static" ammo-shape="type: box"
          position="0 0 -4" rotation="-90 0 0" width="12" height="8"
          color="yellow"></a-plane>

      <!-- Dynamic box -->
      <a-box ammo-body="type: dynamic" ammo-shape="type: box"
          position="-4 4 -2" width=".5" height="2" depth="1"
          color="red"></a-box>
      <!-- Dynamic box -->
      <a-box ammo-body="type: dynamic" ammo-shape="type: box"
          position="-4 5 -2" width="6" height=".2" depth="2"
          color="blue"></a-box>

      <!-- Dynamic box -->
      <a-box ammo-body="type: dynamic" ammo-shape="type: box"
          position="5 4 -2" width=".5" height="2" depth="2"
          color="red"></a-box>
      <!-- Dynamic box -->
      <a-box ammo-body="type: dynamic" ammo-shape="type: box"
          position="2 5 -2" width="7" height=".2" depth="2"
          color="blue"></a-box>
      <!-- Dynamic cylinder -->
      <a-cylinder ammo-body="type: dynamic" ammo-shape="type: box"
          position="2 5 -4" rotation="90 0 0"
          radius=".5" height="1"
          color="green"></a-box>

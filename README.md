# TMP_Billboard-shader
This is the URP version of the Text Mesh Pro Billboard shader. Is a world text that is always facing the rendered camera.
Instead of making complex (and heavy) calculations to present a world-oriented text on screen-space, you can just use this shader to do it and call it done.
This shader is meant to be used in Universal Render Pipeline and will not work on the built in render. I am sure you can easily adapt it to be used on HDRP as well.
A Built in version (that I based my calculations on) is avaliable at https://gist.github.com/Spongert/b52a24aa110933a918cf47c777fea1c8

# Instructions, READ ME!
You HAVE to put his under TextMeshPro/Shaders after importing the TMP essentials
Then you can use it on your materials by looking for it under TextMeshPro/Mobile/TextMesh Billboard by Niter88
The last step is to put this material on the TextMesh Component on a world space canvas

If this code doesn't work in your version of Unity, make a copy of the Mobile Distance Field Shader and Edit like my comments on the code tell you (They all start with "//Niter:")
This doesn't work with an orthographic camera, you can fake the effect using FOV like in https://youtu.be/rnqF6S7PfFA

# Examples of use
You can use this shader to make waypoints, damage numbers on character heads or other kind of UI integrated in 3D space, no worring about distance, size, overlapping, etc.

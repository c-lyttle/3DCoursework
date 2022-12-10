first I worked on compiling the OpenGL template provided, to do so I installed mingw64 which includes the gcc compiler amongst other helpful c++ related tools, this allowed me to run the code, 
After I worked to import my model, the placeholder model (dog.gltf) was a gltf file type and therefore I though it would be wise to render my model from blender as a .gltf instead of trying to importthe model by some other method, blender automatically tried to export as a .gdb which is a .gltf but with the binaries within one file. This isn't what I wanted and I therefore exported it as a .gltf + .bin + textures.
Now I had the model imported I could work on the movement, some basic movement was already implemented along with the key press calbacks, this allowed me to modify the existing code to get panning as well as forward and backward movement.
I used a tutorial on learnopengl.com in order to implement mouse controls for camera movement, this way the camera would be able to freely move around the scene.
Then I wanted to add some interaction by making the gun fire, I did so by rotation the gun frame by frame upon mouse click with the predefined onMouseButtonCallback function.

I was unable to texture my gun as I was unable to successfully get the exported textures to wrap onto the gun model.

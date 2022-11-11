Animation Readme

Export/Import:
At first I tried to export the entire blender file as a .fbx and import into Unreal, this however created a multitude of problems, 1. My pistols weren't displaying correctly, I could see inside them. 2. The lights and camera didn't copy in correctly. 3. Nothing was where it was meant to be in the scene positionally. 4. The materials didnt carry over correctly, only the colours of the materials carried across.

For problem 1 I fixed this back in blender, as I had created the pistols from a plane there was a chance that all the normals had been flipped, this was the case, extruding the wrong side of the plane from the very beginning of the modelcreation has caused the entire model to be inside out. The way I deduced this was by setting the viewport shading to solid, and then within options selecting 'Backface Culling'. This means that backwards faces aren't shown in the viewport and as such my pistols didnt display correctly. To fix this I enterred edit mode, selected the entire pistol and went to Mesh>Normals>Recalculate outside. This fixed the broken normals and now the pistol imported correctly.

Problem 2 was fixed by re-adding cameras and lights within Unreal using their defaults. I wanted a slightly different scene for the animation anyway so adding them back in within unreal was fine.

Problem 3 was fixed by exporting the whole scene as a asingle mesh from within blenders export settings, this meant that everytrhing within my scene was joined together meaning it could simply be placed within the unreal level without issue.

And finally problem 4 was fixed by manually re-adding the roughness ad metallic values to the materials fro within unreal, I also had to completely change the materials for the bottle and fluid within as the translucent glass didnt carry across at all. This however allowed me to play wtht the refractive index of the glass within Unreal which I think made an interestig effect in the final output.

Animations:
In order to animate my scene I used the sequencer and 'level sequence' objects (under the animation drop down) to create different shots for my scene. I keyframed in different points for each shot so that the camera would fly correctly between positions, I also alterred the speed at which the keyframes were reached in order to change the spacing of the video. I then put each of these level sequences into one master level sequence and added a fade track which allowed a 'fade to black' inbetween scenes so that they didnt jump abruptly.

Rendering Settings:
The camera I used for each shot was the 16:9 DSLR as it gave a modern sleek look, as well as having many lenses to choose from, for most shots I used the 50mm lens as it allowed the models to stay in focus for the shots I wanted. I exported in 16:9 also as this is a very common format, and in 1080p as that is the resolution of my monitor at home.

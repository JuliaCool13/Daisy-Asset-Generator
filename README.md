# Daisy-Asset-Generator Documentation
This is a tool I made that can be used to procedurally generate and customize daisies to be put into a game engine. The customizable features include different parameters for the stem, flower head, and leaves. Some of these parameters include stem position, stem thickness, leaf and petal count, and leaf and petal sizes. There are also LODs to switch between for export when customizing the flower. The daisy material was made by me in Substance Designer, and the file of which it was made in is included in the project. The stem's material is simply a basic material with a solid color that I made in Blender.

## How to use the tool:
### 1. Open the "DaisyGen.blend" file
Look at the outliner and look at the "FINAL FLOWER GENERATOR" collection. This is where the tool objects with the tool attached are located. You may also create a new object and add the "DaisyGen" or "Flower Patch" GeometryNodes modifier to make a daisy.

<img width="465" height="312" alt="Screenshot 2026-10-10 000246" src="https://github.com/user-attachments/assets/deed2265-22bb-4ad0-9263-9dacf52d1a0c" />  
  
NOTE: If you do not see the petals on the flower upon adding the "DaisyGen" to a new object, it is because the petal length and width are set to 0 and need to be adjusted.

### 2. The "DaisyGen" parameters:
<img width="459" height="1130" alt="Screenshot 2026-10-10 000326" src="https://github.com/user-attachments/assets/04dba85b-6206-485e-968f-0d83e08173db" /><br/>
#### 1. Flower Position & Rotation:
Used to move and rotate the whole flower.
#### 2. Stem Start, Middle, and End:
Use the XYZ parameters to change the position of the top, middle, and end of the stem. It is recommended to change the height of the flower by using the "Y" parameter of the "Stem Start". It is also recommended to leave the "Stem End" at 0m to leave the flower at a ground position.
#### 3. Stem Thickness:
Changing the thickness of the stem.
#### 4. Stem Detail:
Increasing this number will increase the poly count of the stem to create a more defined shape of the stem.
#### 5. Stem Material:
The stem can be changed to any material. Currently, it is set to "StemColor", which is set on a UV sphere that is kept in the "MaterialTests" collection in the Outliner. Note that the stem is not UV unwrapped.
#### 6. Stem Smooth:
Set stem shade smooth. Uncheck to visibly see the edges of the geometry of the stem/
#### 7. Leaf Scale:
Default is 1.000. It is not recommended to go over 2.5 or go into the negatives for the best results. If the scale is negative, the leaf normals will be flipped.
#### 8. Leaf Length:
Used to change the length of the stem. If you want to scale up or down the leaf with "Leaf Scale" without distorting the UVs, make sure to do the same with the leaf length to keep the same proportions.
#### 9. Leaf Density:
Determines how abundant the leaves are.
#### 10. Leaf Seed:
Randomness of leaf placement.
#### 11. Leaf Rotation Variation and Scale Variation:
Changes the strength of variation in rotation and scale of the leaves.
#### 12. Leaf Material:
The leaves can be changed to any material. Currently, it is set to "DaisyMAT", which the UVs of the leaves have been set in the correct position for. If you change the material, it is possible the UVs need to be changed. To change the UVs, you will have to go into the "DaisyGen" geometry nodes to adjust them.
#### 13. Petal Count:
Changes the number of vertices on the circle of the flower head, which changes the number of petals seen.
#### 14. Petal Length and Width:
If you do not see the petals on the flower upon adding the "DaisyGen" to a new object, it is because the petal length and width are set to 0 and need to be adjusted.
#### 15. Petal Material:
The petals can be changed to any material. Currently, it is set to "DaisyMAT", which the UVs of the petals have been set in the correct position for. If you change the material, it is possible the UVs need to be changed. To change the UVs, you will have to go into the "DaisyGen" geometry nodes to adjust them.
#### 16. Center Flower Head Material:
The center flower head can be changed to any material. Currently, it is set to "DaisyMAT", which the UVs of the head have been set in the correct position for. If you change the material, it is possible the UVs need to be changed. To change the UVs, you will have to open the "Flower Parts" collection in the Outliner, and move the UVs of the "YellowCenter" object.
#### 17. Flower Head Scale:
Used to change the scale of the flower head.
#### 18. Realize Instances:
This makes the instances on the flower (like the leaves, petals, and heads) real geometry. It is important to leave this checked when making the flower patch to improve performance.
#### 19. Flower LOD:
There are 5 different LODs, with level 0 being the highest poly, and level 4 being the lowest poly.

### 3. The "Flower Patch" Parameters
<img width="462" height="465" alt="Screenshot 2026-10-10 000347" src="https://github.com/user-attachments/assets/d644117a-e0f4-4c4d-b81f-377c078402f4" /><br/>
#### 1. Seed:
Randomizes the placement of flowers.
#### 2. Random Rotation:
Randomizes the rotation of the flowers.
#### 3. Object Collection:
This determines what specific objects are placed down. It is taking from a collection called "Flower Collection". To have your own flowers in this collection, make sure to add them to it in the Outliner, or make your own collection and set it in the "Object Collection" setting.
#### 4. Flower Density:
Determines the number of flowers placed on the patch.
#### 5. Patch radius:
Changes the size of the flower patch.
#### 6. Realize Instances:
This makes the instances of the flower patch (all of the flowers placed) real geometry. It is important to leave this checked when applying the modifier and exporting the flower patch.
#### 7. Flower Patch LOD:
There are 5 different LODs, with level 0 being the highest poly, and level 4 being the lowest poly. It is recommended that the individual flowers are set to an LOD of 0 before changing the flower patch LOD.


## Special thanks to these resources for helping me in creating this project:
- For using splines to create a leaf shape in Substance Designer: https://www.youtube.com/watch?v=VehiwgvCbVg
- Procedural shapes in Substance Designer: https://www.youtube.com/watch?v=_tLjvmGcEcc&list=PLB0wXHrWAmCxBw92VSRjqsbqYXgkF8puC&index=8
- A great walkthrough for creating foliage in Substance Designer: https://www.youtube.com/watch?v=cCZgMfQMKU0
- Awesome tutorial series for creating a flower with geometry nodes: https://youtube.com/playlist?list=PLsGl9GczcgBsDZ3jQPwP1p6evNI22wevP&si=EXLacGqhia86vSa_
- Rotating and flipping around UV faces: https://blender.stackexchange.com/questions/333988/how-can-i-flip-rotate-uv-faces-around-with-geometry-nodes


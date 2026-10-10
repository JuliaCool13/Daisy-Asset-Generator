# Daisy-Asset-Generator Documentation
This is a tool I made that can be used to procedurally generate and customize daisies to be put into a game engine. The customizable features include different parameters for the stem, flower head, and leaves. Some of these parameters include stem position, stem thickness, leaf and petal count, and leaf and petal sizes. There are also LODs to switch between for export when customizing the flower. The daisy material was made by me in Substance Designer, and the file of which it was made in is included in the project. The stem's material is simply a basic material with a solid color that I made in Blender.

## How to use the tool:
### 1. Open the "DaisyGen.blend" file
Look at the outliner and look at the "FINAL FLOWER GENERATOR" collection. This is where the tool objects with the tool attached are located. You may also create a new object and add the "DaisyGen" or "Flower Patch" GeometryNodes modifier to make a daisy.

<img width="465" height="312" alt="Screenshot 2026-10-10 000246" src="https://github.com/user-attachments/assets/deed2265-22bb-4ad0-9263-9dacf52d1a0c" />

### 2. The "DaisyGen" parameters:
<img width="459" height="1130" alt="Screenshot 2026-10-10 000326" src="https://github.com/user-attachments/assets/04dba85b-6206-485e-968f-0d83e08173db" />

--------------------------------------------------------------------------------------------------------------------------

1. Flower Position:
- 


NOTE: If you do not see the petals on the flower upon adding the "DaisyGen" to a new object, it is because the petal length and width are set to 0 and need to be adjusted.

<img width="462" height="465" alt="Screenshot 2026-10-10 000347" src="https://github.com/user-attachments/assets/d644117a-e0f4-4c4d-b81f-377c078402f4" />


## Special thanks to these resources for helping me in creating this project:
- For using splines to create a leaf shape in Substance Designer: https://www.youtube.com/watch?v=VehiwgvCbVg
- Procedural shapes in Substance Designer: https://www.youtube.com/watch?v=_tLjvmGcEcc&list=PLB0wXHrWAmCxBw92VSRjqsbqYXgkF8puC&index=8
- A great walkthrough for creating foliage in Substance Designer: https://www.youtube.com/watch?v=cCZgMfQMKU0
- Awesome tutorial series for creating a flower with geometry nodes: https://youtube.com/playlist?list=PLsGl9GczcgBsDZ3jQPwP1p6evNI22wevP&si=EXLacGqhia86vSa_
- Rotating and flipping around UV faces: https://blender.stackexchange.com/questions/333988/how-can-i-flip-rotate-uv-faces-around-with-geometry-nodes


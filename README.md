# OpenGL Tutorial


## Transformation
Translation Matrices
```
1 0 0 X
0 1 0 Y
0 0 1 Z
0 0 0 1
```

Identity Matrices
```
1 0 0 0
0 1 0 0
0 0 1 0
0 0 0 1
```
 
does not do anything, but it's important to know multiply this will give the original matrix

Scalling Matrices
```
X 0 0 0
0 Y 0 0
0 0 Z 0
0 0 0 1
```

Rotation Matrices
```
glm::vec3 myRotationAxis( ??, ??, ??);
glm::rotate( angle_in_degrees, myRotationAxis );
```
it's not clear yet how rotation works behind the scene

## Pipeline
      - Vertex -> Fragment
      - Bind different buffer to draw different object in the main loop, remember to call attribute pointer function again.
      - Buffer data need to be updated in order to change color in the main loop.
      - Only the last gl_position assighment will be effective.


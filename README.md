Reference: https://youtu.be/Ec_48EEkMgU?si=s4t1kCSJ7FuYPoV_ 

Video of what it looks like: [https://youtu.be/VvajVVVfCeI ](https://youtu.be/zXbxenSrcl0)

Shader Graph

<img width="1338" height="589" alt="image" src="https://github.com/user-attachments/assets/cd7a8af5-4812-440c-86c4-7d2b634b7ed7" />

I Chose to try to recreate the mosaic slime from Slime Rancher

So the first effect is the outer glass shell, created by the "noise set up group". This takes voronoi noise and then add an exponent in order to 
sharpen the edges. This creates the edges of our glass and is used add a white border to the glass as well a creating a bump map. 

The second effect is the rainbow slime. I wanted it to be red in the middle then go through the colors of the rainbow. I did this by having
a gradient that when through the rainbow and deciding the color value off of the dot product of the normal vector and view direction. Using
the normal vector here, it ends up creating a sort of light refracting effects.

The 0 value for the gradient is also black. I did this so I could plug the color into the alpha so that the black would be transparent.
This is what gives us that encased look that there is a gap between the outer glass and the inner slime.

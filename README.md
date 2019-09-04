The Odin Project - Project - Etch-a-Sketch

1. Create a webpage with a 16x16 grid of square divs
2. Set up a “hover” effect so that the grid divs change color when your mouse passes over them, leaving a (pixelated) trail through your grid like a pen would. 
3. Add a button to the top of the screen which will clear the current grid and send the user a popup asking for how many squares per side to make the new grid. Once entered the new grid should be generated in the same total space as before (e.g. 960px wide) and now you’ve got a new sketch pad. 


Learnings: 

var gridContainer = document.getElementById("container");

The above only needs to get called once as the container is never deleted, while the querySelectorAll in hoverAction() needs to be redeclared(nested) as all existing divs (that had been selected initially) were removed during reset.
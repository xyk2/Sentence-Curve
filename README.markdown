Sentence to Curve Generator
---------------

 Enter any phrase or sentence and the program will convert and draw those into curves.  
 
 The program flow is like this:  
 Collect entered data -> parse ASCII string into integers and store in array -> draw random bezier curves from values in that array.  

Each ASCII symbol (letters, periods, spaces, numbers.. etc) is paired with a decimal value that is determined with the int() function.
 Try to enter more than ~20 characters for varied curves (internal limit of 100 to avoid hogging resources).  
 

There is an inherent issue with the method of animating beziers: since the animation is a just bunch of little circles moving on the path, they will ocassionally split up as the speed increases.  
This problem can be improved by changing variable ballSpeed, which controls how many ellipses are drawn (1/ballSpeed is the number of ellipses). This will slow the animation down, however.  
 

###Future improvements:
- Animate more than one curve at the same time (requires many arrays which is too complicated at the moment)  
- fix ball-separating issue  
- reverse-fade when alpha is at max  
- backgrounds   
- change color, different shapes  
- draw text of input along the bezier curves (atan2/bezierTangent)
 
 
###User-controllable variables:
- ballSpeed - speed of ball (indirectly controls density of ellipses)  
bezierCountMax - maximum number of beziers before sketch stops (preset at 30)  
- The checkbox at the start screen lets you choose whether you want to display the bezier curve or not  
- The second checkbox lets you select whether you want fading or not
 The slider lets you select how many curves to draw  




**Licensed under a [Creative Commons Attribution-Non Commercial-Share Alike v3.0 license.]**

  [Creative Commons Attribution-Non Commercial-Share Alike v3.0 license.]: http://creativecommons.org/licenses/by-nc-sa/3.0/
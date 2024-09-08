# csci5611-project1

Group members: Zhipeng and Ekin 

Pinball project

Videos:

https://github.com/user-attachments/assets/1e1ea9fd-e055-4b26-99bb-7b1d6def00c4





Features attempted:  
1.	basic pinball dynamics. The ball could fall down and nature bouncing with other obstacles. When press r pinball would back to position.  
2.	multiple balls interacting. The pinballs would have natural collision and bouncing with each other.  
3.	circular obstacles. The pinball would interaction with circular obstacles would be natural and smooth without getting into the circle.  
4.	line segment and polygon obstacles. The circle would not cross the line when perpendicular to the line and would not move pass it. Same for the polygon.  
5.	launcher to shoot balls. With pressing two times down, or not, the launcher would launch two balls on the platform at a speed of 5. It would always back to initial position automatically.   
6.	textured background. Import a star filed  
7.	textured obstacle. Circle import aliens, rectangle import space crafts,  hexagon import twill image. Launcher import falt aliens ship. Line with specific color  
8.	reactive obstacles. The line would change color to yellow when the pinball collides with it permanently during the game. Pressing r would bring the line back to     purple   
9.	multiple material types. The ball would bounce back with different velocities with different obstacles. Details in collision_lib.pde 1-5 lines.   
10.	loading scenes from the file, have a reading file method from file to read the coordinates of all objects.   
11.	complete the pinball game with flippers. Could bouncing the ball with rotational velocity and the point of impact. The game could track the player score and support multiple balls and when all balls touch the bot line game would end.   
code written by us:   
Zhipeng: wrote the main part for collision lib (including multiple ball interaction, circular obstacles, circle box collision, circle hexagon collision, and circle line collision) and added on for vec2. Adding textured obstacles, adding hexagon classes, adding multiple material types, and reactive obstacles.  
Ekin: working on the part for flippers class, and ball flipper collision in collision lib. Adding animation for ball back to the animation.  
List of tools:  
We used the flipper code provided by professor Steven Guys vec 2 lib. P2D engine in processing   
Difficulties we encountered:  
When the ball speeds up, sometimes the ball easily passes through the line and other obstacles, and the same for the flipper. For flippers, we tried the code provided by Steven and did a physics simulation, for obstacles, we tried adding time steps method for this.     
For the launcher, we have problems with how the launcher moves back smoothly, we added an acceleration for the box moving back or up or down. When u press the upper or down key longer the speed would decrease to 0; when you release the key it would back with normal speed. We tried to draw a spring but we found that it was not   efficient, why not have a moving box that would bounce the ball with velocity 5? Which just need to a true false evaluation for box to determine whether the box could move.  
To import the texture into the hexagon, we figured out we had to use P2D engine provided by processing, then we could fill the image with a map and transform into the hexagon. 

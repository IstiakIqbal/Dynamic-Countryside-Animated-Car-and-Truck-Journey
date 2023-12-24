This project brings a peaceful countryside scene to life using computer graphics. It showcases nature's beauty with trees, bushes, flowers, and a road where cars and trucks are on their journey all under a lovely sky.
By combining simple shapes and vibrant colors, it crafts a serene environment. Animated elements like drifting clouds and moving vehicles add a realistic touch, making the scene come alive. One interesting feature is the small interaction it offers - users can move the clouds using keyboard keys, adding a fun twist to the experience.

Through colors and details, it aims to capture attention and create an engaging visual story of a tranquil countryside setting. It merges technology and creativity, offering a delightful digital portrayal of nature's charm.


Code explanation(segment wise)

●	Drawing functions for rounded object
❖	Functions: circle() and round()
❖	Purpose: These functions define how to draw circles and rounded shapes using OpenGL.
❖	Usage: They calculate the vertices of shapes based on given parameters like radius and center coordinates.

●	Initialization function
❖	Function: init()
❖	Purpose: Sets up the initial state for OpenGL.
❖	Usage: Configures background color and sets the viewing area for the graphics window.

●	Drawing functions for scene or countryside elements
1.	Bushes():
❖	Purpose: Draws bushes in the landscape.
❖	Usage: Utilizes the circle() function to create circular shapes representing bushes. Multiple circles are drawn with different positions and colors to form the bushes.
2.	road():
❖	Purpose: Constructs the road with lanes and dividers.
❖	Usage: Uses GL_POLYGON to draw the road, car lanes, and dividing stripes. It employs multiple GL_POLYGON calls to create the different segments of the road.
3.	sun(), tree(), little_tree():
❖	Purpose: Each function draws a specific element like the sun, trees, smaller trees, flowers, etc.
❖	Usage: Utilizes various shapes and polygons (often circles) drawn with appropriate colors to represent these elements in the scene.


●	Animation Functions for creating motion
1.	clouds2():
❖	Purpose: Animates the clouds' movement across the sky.
❖	Usage: Utilizes glPushMatrix() and glPopMatrix() to translate the cloud shapes, creating the effect of clouds moving horizontally. Continuously updates the cloud positions for animation.
2.	car(), truck():
❖	Purpose: Manages the movement and animation of the car and truck.
❖	Usage: Uses glPushMatrix() and glPopMatrix() to translate the car and truck shapes, simulating their movement across the screen. Continuously updates their positions for animation effect. Inside these functions the speed of the car and the truck can also be increased and decreased according to the user’s desire.

●	Function for displaying 
❖	Function: display()
❖	Purpose: Draws the entire countryside scene by calling various drawing functions.
❖	Usage: Utilizes other drawing and animation functions to display the complete landscape on the screen.

●	Keyboard interaction function
❖	Function: key()
❖	Purpose: Manages keyboard inputs, specifically arrow keys.
❖	Usage: Allows users to interact with the scene by moving the clouds horizontally using arrow key inputs.

●	Main function (entry point)
❖	Function: main()
❖	Purpose: Entry point of the program, manages program execution.
❖	Usage: Initializes GLUT, sets up the window, associates display and interaction functions, and starts the program loop to maintain the window and its functionalities.

This code blends drawing functions, animation techniques, user interaction, and program execution to create a countryside landscape visualization with animated elements such as moving clouds, a car, and a truck.

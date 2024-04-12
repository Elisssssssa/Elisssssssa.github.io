Pumpkin-Platform-Game
========================================
![main page](https://user-images.githubusercontent.com/115221489/229107711-c478b92c-2d40-4a3b-b41a-e952330273f5.PNG)

Special about this game
------------------------------------

  * Three enemies
  * Some life pumpkins
  * Some poison pumpkins
  * Swamp(slow speed)
  * Glass platform
  
How to win this game?
------------------------------------

  Control the player to  get the sun flower to win.
  
Code to make Glass Platform
----------------------------------
  * When the player is touching the platform
~~~python
elif self.is_touching_any_sprite_with_tag('glass'):
            glass.image = 'glass2.png'
            Scheduler.wait(0.5,glass.fall)
        if glass.can_fall == True:
            glass.image = 'brokenglass.png'
            glass.scale = 0.5
            glass.rotation = 180
            
~~~
  * After 0.5 second the platform changes the boolean to True to fall down
  ~~~python
  class Glass(Sprite):
      def on_update(self, dt):
        if self.can_fall == True:
            self.speed.y -= 0.5
            self.position += self.speed 
        if self.is_touching_any_sprite_with_tag('ldtk_Ground'):
            self.can_fall = False
            self.tags.clear()
            while self.is_touching_any_sprite_with_tag('ldtk_Ground'):
                self.y += 1
            self.image = 'brokenglass.png'
            self.speed.y = 0
            self.delete()
         
~~~ 

The webside that used in this game
-------------------------------------

  * [Python](https://www.python.org/)
  * [VS Code](https://code.visualstudio.com/)
  * [Kenny Assets](https://www.kenney.nl/assets)
  * [Ldtk](https://ldtk.io/)
  * [Google(search the picture)](https://www.google.com/search?gs_ssp=eJzj4tTP1TcwMU02T1JgNGB0YPBiS8_PT89JBQBASQXT&q=google&rlz=1C1GCEA_enTW855TW855&oq=Goo&aqs=chrome.1.69i57j46i67i199i465i650j0i67i650l5j5.2666j0j7&sourceid=chrome&ie=UTF-8)

Video
---------------------------------

<video src="https://user-images.githubusercontent.com/115221489/229121825-8a65b334-4f6c-4ac7-a43a-f85b0f6b21e4.mp4" controls="controls" style="max-width: 730px;">
</video>






Earth Lander
========================================            
            
[Play!](Elissa_Earth_lander_webgl_v2/index.html) 

Special about this game
------------------------------------

  * Only use three key to control the lander
  * Two enemy rocket
  * Land on the Earth in perfect speed and right rotation
  * Very hard!!!

How to win this game?
------------------------------------

  Control the player lander to land on Earth perfectly, 
  it means you have to let the lander land slowly on the Earth, 
  and also keep the rotation of the lander in 20.


  
Maze
========================================                   
[Play!](Elissa_maze_webgl4/index.html) 

Things to prepare in this game
------------------------------------

* Build the maze(easy but takes a long time)
* Player
* Pickup
* Mission
* Door
* Obstacle(make the game more difficult)


Special about this game
------------------------------------

* 3D Game
* First Perspective(can make you feel that you are inthe real maze)
* Math Mission
* Obstacle
* Exciting!!!
  

How to win this game?
------------------------------------
* Find the exit of the maze(you will see a bed right there).
* Don't let your life be less than 0 or you will be back to the original point.


Favorite part
------------------------------------
Math mission and Pickup

Hardest part
------------------------------------
Math misssion



Clicking_Game
================================================
[Play!](clicking_game_webgl/index.html) 



Tower_shooting
================================================
[Play!](Tower_shooting_webgl1/index.html) 


Running_guy
================================================
[Play!](Running_guy_webgl1/index.html) 

Play_tag
================================================
[Play!](Play_tag_webgl2/index.html) 

Ball_Puzzle
================================================
[Play!](BallPuzzle_webgl2/index.html) 

Block_Pushing
================================================
[Play!](Block_pushing_webgl1/index.html) 



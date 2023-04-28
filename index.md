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

# Racing-AI
How to import the Racing AI into eclipse. (Created by Till Roßberg at the HTW, 2017)
1. Unzip the file.
2. Create an empty Eclipse Java Project.
3. Import all the data from the RacingAI.zip into the new project.
   (RMB on the project->Import...chose 'Archive File' from folder 'General', then browse for 'RacingAI.zip'.)
4. Add the .jar-files to the build path of the project. 
   (RMB on the project-> Buildpath-> configure buildpath...-> Add External JARs...[on the right side in the libraries tab]
   chose ai.jar and ai_libs.jar from the 'Required Data' folder.)
5. Under 'ai_libs.jar' chose 'Native library location'-> Edit...-> External folder then chose the native folder from the 'Required Data' folder.
6. Create a new run configuration in the Run Configurations Window (Run-> Run Configurations-> the small white sheet with the plus on it)
7. In the 'Main' tab select as main class 'lenz.htw.ai4g.Simulator'.
8. In the 'Arguments' tab set as program arguments 1024 786 13. (The first two numbers are the resolution, followed by the track number.
   Possible are tracks 10-13 and 20,21,30 and 31, increasing difficulty with number.)
9. Run as Java Application! 

Hopefully it all works!

The green lines indicate possible connections between the waypoints and the edges of the obstacles,
the white line shows the path to the next waypoint and the blue line indicates the velocity. I inserted the 'Dummy'
so the camera doesn't stay fixed on the car and the track is better visible.


Enjoy! :)

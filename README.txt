Developed by Unreal Engine 4.18.2
by: Katax

Katax.emperor@gmail.com
www.linkedin.com/in/cliff-sharif/ 

This application spawned number of static meshes into the stage and, when character collisions with them, each send unique message to game mode class and destroy themselves. This message appears on “Output log” in editor at the moment but can be used for Spawn other static objects or maybe time-based particle system to present destruction effect.
All classes purely developed and are functional with Blueprint.
 BP_GeoSpawner class, is responsible for spawn static meshes in number. User can change maximum shape number and also assign collision object. Shapes are made by BP_Sphere class and they get destroyed when they overlapped by collision object which here in this sample is set to third person character as default. Also, shape will send message to Game Mode class before destruction. This message shows their name, id and parent class name which comes up in output log. This message can be customised by user based on requirements. 
Indeed, BP_Sphere is not using any “event dispatcher” for send message.

note: This sample of application shows 3 walls made from number of static meshes which are made by 3 BP_GeoSpawner classes. Total number of meshes are 320 spheres and they respond to player character movement. On collision with character, they will show message in output log and destroy. For make new wall, drag an “BP_GeoSpawner” class into the scene, change its “Transform” scale and positions, set up “Maximum Items” and finally set “CollisionObjectClassName” to your preferred name. Click play and run through the new wall, also check output log for details.


Cheers … ; ] ,,,

# RamsHornMobileVR

This was a WebXR experiment I made as part of the VRPlants research project at North Carolina State University. Over the course of my involvment with the project I learned to use the *A-Frame* WebXR framework and write components to make unique experiences.

This experience is focused around the Ram's Horn seed pod, which has tusk-like barbs that allow it to attach to fauna and propogate. In this experience, the user tries to lob 3D scans of the seed pod to latch them onto bison that mill around the space; attaching 5 to a single bison makes the seed pods detatch and despawn. Future iterations could add baked particle effects using an existing *A-Frame* component, explore geometry instancing to render more detailed bison (we were conflicted on detailing the fauna further in a flora-focused experience), and add further gamification like scoring, time limits, etc.

Some components I created include:

- "Sticky" component that keeps track of physics objects of a certain class in the scene and "attaches" them to the surface of the object when they collide. Developers can specify the class type to "stick", as well as the number of objects that stick before they are released. An event can also be fired to manually release the "sticking" objects.
- "Spawner" component that creates copies of physics object when user passes VR hand through preview mesh and "grabs" (this isn't featured in this demo but in a previous Oculus-Rift-focused version)
- "Launcher" component that lets users on mobile launch seed pods from the camera by touching and holding touch screen to "charge" and releasing to "throw". When using a Google-cardboard-like smartphone headset, users can perform this action by using the "trigger" button on the top of the assembly.


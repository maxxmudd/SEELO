# SEELO
C#, Unity, Python, Blender Git, GitLab - Coded in 2021. This repository describes my work as an intern for NASA Kennedy Space Center's SEELO Project.

[TechPort: Simulated Excavation Environment for Lunar Operations (SEELO)](https://techport.nasa.gov/projects/117509)

[NTRS: Simulated Excavation Environment for Lunar Operations](https://ntrs.nasa.gov/citations/20220018679)

From May 2021 to December 2021, I was a software developer intern for the Simulated Excavation Environment for Lunar Operations (SEELO) project at NASA's Kennedy Space Center. SEELO was a research tool developed in Unity engine to give engineers a testing environment for CAD-modeled rover designs, with the purpose of gaining insight into their performance on the lunar surface. The simulation included microgravity and regolith physics, generation of lunar terrain based on lunar orbiter data, modeling of collision physics for understanding the effects of long-term excavation, all wrapped withhin a user-friendly UI. This project was part of a research initiative for the Artemis program, an initiative to return to the Moon and identify water sources near Shackleton crater.

In SEELO's initial phase, I was in charge of creating the software's terrain generation system. This feature involved an automated process of pulling heightmap images from the Lunar Reconnaissance Orbiter, translating 16-bit grayscale pixel values in a square area based on lunar coordinates, and assigning those values to vertices on a 3D plane in Blender to import as a model into Unity. Blender's Python interpreter allows Python scripts to interact with its functionality, enabling the generation of objects with specified attributes. Through the UI in Unity, coordinates were parsed, which could then be searched against lunar orbiter data collection. The identified area was recreated using the Python-Blender pipeline, and was imported into Unity as a GameObject, all occurring during the software's runtime.

The result of this work allowed the recreation of any location on the lunar surface by simply entering lunar coordinates. This allowed engineers to test their rovers against various features of the lunar surface, including planes, hills, craters, or any other feature that was desirable to explore.

Towards the end of my internship, my tasks involved learning the Unity Test Framework (UTF) and implementing comprehensive unit tests to ensure functionality was protected across the many code changes in our collaborative coding environment. As complex features were added, it was critical to maintain functionality across updates to the code base. At the start of runtime, Unity would run these tests to ensure features were functioning as intended, generating errors to notify the team of broken components, or proceeding with the simulation if the expected outcomes were produced.

This work resulted in a more reliable code base and prevented regressions from occurring, while also notifying the team of broken features that could be patched immediately.

All contributions on this project are property of the U.S. Government/NASA and were created on a private GitLab repository. For more information, please contact me.

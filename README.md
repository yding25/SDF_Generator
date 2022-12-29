# SDF_Generator


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PiPWuaiH2tcx8PpW7rUIuncVwmL6Hyg9?usp=sharing)  

The author has used [Gazebo-models-generator](https://github.com/TurtleZhong/Gazebo-models-generator) for reference. **SDF_Generator** is for generating 3D object models (*sdf) in Gazebo with taking *.obj / *.dae as input. Different from Gazebo-models-generator, SDF_Generator can 

   - preprocess mesh files, 
   - handle *.dae files, 
   - consider inertia matrix,
   - add different colors to models. 

<br/>

❤️ ❤️ ❤️ If one does not want to build SDF models from scratch, they can freely download models from another project [SDF_Models](https://github.com/yding25/SDF_models).

<br/>

✨✨✨ **Tips**: 

- Sources to download mesh files (*.obj/*dae) of an object.
   - [turbosquid](https://www.turbosquid.com/)
   - [cgtrader](https://www.cgtrader.com/)
   - [free3d](https://free3d.com/)
   - [3dwarehouse](https://3dwarehouse.sketchup.com/)
   - [gazebosim](https://app.gazebosim.org/fuel/models)
   - [sketchfab](https://sketchfab.com/feed)
  
- [Blender](https://www.blender.org/) and [Sketchup](https://www.sketchup.com/) can convert other formats (*.3DS) into *.obj / *dae. 
 
- It is better to [set origin to center of mass](https://docs.blender.org/manual/en/3.4/scene_layout/object/origin.html#bpy-ops-object-origin-set).
 
 
<br/>

✨✨✨ **References**: 

- [How to add customized model in Gazebo (in chinese)](https://blog.csdn.net/NEUer_ljx/article/details/125504848?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-0-125504848-blog-98712486.pc_relevant_landingrelevant&spm=1001.2101.3001.4242.1&utm_relevant_index=3)

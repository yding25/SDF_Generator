# SDF_Generator

This project is forked from [Gazebo-models-generator](https://github.com/TurtleZhong/Gazebo-models-generator). Thanks for the author's efforts.

**SDF_Generator** is for generating 3D object models (*sdf) in Gazebo with taking *.obj / *.dae as input. Different from Gazebo-models-generator, SDF_Generator is able to preprocess mesh file, and to automatically handle *.dae files. Besides, if one does not want to build SDF models, he/she can freely download models from my another project [SDF_Models](https://github.com/yding25/SDF_models).

**SDF_Generator** consists of three steps:
- **Step 1**: Download mesh file (*.obj/*dae) of an object. Here are some sources: 
    - [turbosquid](https://www.turbosquid.com/)
    - [cgtrader](https://www.cgtrader.com/)
    - [free3d](https://free3d.com/)
    - [3dwarehouse](https://3dwarehouse.sketchup.com/)
    - [gazebosim](https://app.gazebosim.org/fuel/models)
  
  **!!!** Note that softwares (e.g., [Blender](https://www.blender.org/) and [Sketchup](https://www.sketchup.com/)) can convert other formats (*.3DS) into *.obj / *dae. Here, details are skipped.

- **Step 2**: Clean mesh files using [Mesh Cleaner](https://www.hamzamerzic.info/mesh_cleaner/), and download the new mesh files.
  
<p align="center">
  <a href="">
    <img src="images/mesh_cleaner.png" alt="[Logo]" width="70%">
  </a>
</p>

- **Step 3**: Convert mesh files to *SDF using scripts
```bash
git clone https://github.com/yding25/SDF_Generator.git
cd SDF_Generator
python sdf_generator.py --model_name=YOUR_MODEL_NAME
```
**!!!** Note that **YOUR_MODEL_NAME** is from YOUR_MODEL_NAME.obj or YOUR_MODEL_NAME.dae downloaded from Mesh Cleaner.

- **Step 4**: Edit the generated *.SDF file
  - by changing ```<static>true</static>``` to ```<static>false</static>```
  - by adding the inertia matrix (obtained in Step 2: Mesh Cleaner)
      <p align="center">
        <a href="">
          <img src="images/final_sdf.png" alt="[Logo]" width="70%">
        </a>
      </p>

- **Step 5**: Move/Copy *SDF to ~/.gazebo/models/
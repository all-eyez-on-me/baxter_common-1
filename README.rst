birl_baxter_common
===================

URDF, meshes, and custom messages describing the Baxter Research Robot from Rethink Robotics , Improving by BIRL. This package is suitable for birl Baxter Robot research.

Code & Tickets
--------------

+-----------------+----------------------------------------------------------------+
| Documentation   | http://sdk.rethinkrobotics.com/wiki                            |
|                 | https://github.com/birlrobotics/birl_baxter/wiki               |
+-----------------+----------------------------------------------------------------+
| Issues          | https://github.com/RethinkRobotics/baxter_common/issues        |
+-----------------+----------------------------------------------------------------+
| Contributions   | http://sdk.rethinkrobotics.com/wiki/Contributions              |
|                 | https://github.com/birlrobotics/                               |           
+-----------------+----------------------------------------------------------------+

baxter_common Repository Overview
---------------------------------

::

     .
     +-- robots_description       baxter urdf and meshes for birl baxter research
     |   +--config
     |   +--easy_launch               use this launch file if you are beginner
     |   +--launch                    launch file for user who is familiar with baxter urdf
     |   +--robots                    some urdf for table and camera with baxter
     |   +--urdf                      some urdf for table and camera
     |   +--meshes                    some meshes for table and camera
     +-- baxter_common/           baxter_common metapackage
     |
     +-- baxter_description/      urdf and meshes describing baxter
     |   +-- urdf/
     |   +-- meshes/
     |
     +-- baxter_core_msgs/        messages and services for communication with baxter
     |   +-- msgs/
     |   +-- srvs/
     |
     +-- baxter_maintenance_msgs/ messages for baxter maintenance routines
     |   +-- msgs/
     |
     +-- rethink_ee_description/  urdf and meshes describing end effectors
     |   +-- urdf/
     |   +-- meshes/


Other Baxter Repositories
-------------------------

+------------------+-----------------------------------------------------+
| baxter           | https://github.com/RethinkRobotics/baxter           |
+------------------+-----------------------------------------------------+
| baxter_interface | https://github.com/RethinkRobotics/baxter_interface |
+------------------+-----------------------------------------------------+
| baxter_tools     | https://github.com/RethinkRobotics/baxter_tools     |
+------------------+-----------------------------------------------------+
| baxter_examples  | https://github.com/RethinkRobotics/baxter_examples  |
+------------------+-----------------------------------------------------+
| birl_sensors     | https://github.com/birlrobotics/birl_sensors        |
+------------------+-----------------------------------------------------+

Latest Release Information
--------------------------

   http://sdk.rethinkrobotics.com/wiki/Release-Changes

   https://github.com/birlrobotics




Improvement by Ben for birl Baxter
--------------------------------

1.Improvement in files

::

   we improve the launch files, urdf files, mesh files.
   
   .
   +--robots_description
   |  +--easy_launch
   |  +--launch
   +--rethink__ee_description
   |  +--urdf
   |     +--electric_gripper
   |     |  +--forcesensor_full2.URDF
   |     |  +--rethink_electric_pa_gripper.xacro
   |     +--sake_gripper
   |  +--meshes
   |     +--electric_pa_gripper_base.stl
   |     +--female_camera
   |     +--forcesensor
   |     +--electric_gripper_base.stl
   +--baxter_description
   |  +--urdf
   |     +--left_end_pa_effector.urdf.xacro
   |     +--right_end_pa_effector.urdf.xacro
   |     +--baxter_ft2.urdf.xacro
   |     +--baxter_full.urdf.xacro
   |     +--baxter_sake.urdf.xacro
   |     +--baxter_base
   |        +--baxter_base_ft2.urdf.xacro
   |  
   |

2.Improvement in model

      improving the model of forcesensor, sakegripper, camera frame, male camera both in rviz and gazebo


birl baxter run
----------------------

if you are the beginner,try this
::

     roslaunch robots_description baxter_rviz_r_ft_camera.launch
          or
     roslaunch robots_description baxter_gazebo_r_ft_camera.launch

if you are user who is familiar with baxter urdf
::
   
     roslaunch robots_description baxter_rviz_full.launch
          or
     roslaunch robots_description baxter_gazebo_full.launch


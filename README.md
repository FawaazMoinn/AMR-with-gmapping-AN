# AMR-with-gmapping-AN

![image](https://user-images.githubusercontent.com/69638726/199431394-997829b5-a4f2-4ce5-9868-8ac99fcd445a.png)

A 4-wheeled mobile bot which autonomously navigates while mapping the environment with gmapping SLAM algorithm and partile filter algorithm viz AMCL(Adaptive Monte Carlo Localization) whose URDF is created in Fusion 360 below image:

## URDF Image created in Fusion 360

![amr v2](https://user-images.githubusercontent.com/69638726/199487703-2b231099-0af6-4f19-b35f-5aa28df56436.png)

## To launch model in Gazebo 

Enter the command in Terminal

```roslaunch amr_description gazebo.launch```

![image](https://user-images.githubusercontent.com/69638726/199502221-00fe4908-5dda-4332-ad69-1c0cbe4cd3f2.png)

here you can explore the gazebo environment 

To control bot using keyboard, enter in the new terminal:

```rosrun teleop_twist_keyboard teleop_twist_keyboard.py```

## To launch model in Rviz with AMCL localizer and move_base pkg

enter the command in new terminal:

```roslaunch amr_description an.launch```

rviz and gazebo will open with below visual:

![image](https://user-images.githubusercontent.com/69638726/199504404-4d887883-48e9-401d-a7ad-bb8b07a32829.png)


It is clear that amcl localization is scattered you move bot using teleop twist send a goal command to localize the robot while simultaneously autonomously navigating

![image](https://user-images.githubusercontent.com/69638726/199505532-70f89e8f-906a-4d93-8452-0d6c84bd43bc.png)


![image](https://user-images.githubusercontent.com/69638726/199505581-174d2870-bfb8-40ab-afb0-8e631308a04e.png)





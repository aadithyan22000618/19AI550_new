Ex.No: 4 Create a player Movement Script in unity

REGISTER NUMBER : 212222230001

AIM:
To write a program to create a player movement in unity.

Algorithm:
Create a New Unity Project by Open the Unity Hub and create a new 3D Project,Name the project (e.g., PlayerMovement).

Create the Moving Object In the Hierarchy, right-click → 3D Object → Capsule (or Sphere). Rename it to Player

Adding the Player Movement Behavior Script Create the Script-In the Project Window, go to the Assets folder. Right-click → Create → C# Script.

Write a script for player behavior and save it

Attach the Script Select player in the Hierarchy - Drag & Drop the playerBehavior script onto the Inspector Panel.

Run the game

Stop the program

Program:
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Player_movement : MonoBehaviour
{
    public float speed = 5.0f;

void Update()
{
    float xdir = Input.GetAxis("Horizontal") * speed * Time.deltaTime;
    float zdir = Input.GetAxis("Vertical") * speed * Time.deltaTime;

    transform.Translate(xdir, 0, zdir);
}
}

OUTPUT 
![image](https://github.com/user-attachments/assets/59c9e71a-74b9-41ba-aa45-fae50bdf4933)
![image](https://github.com/user-attachments/assets/5d1f17b8-7a79-443f-82f0-3dc11a9433ae)
![image](https://github.com/user-attachments/assets/b45c3d5d-ec3a-4268-8b6e-4e870c712f49)
![image](https://github.com/user-attachments/assets/a02b6638-9d55-487a-b6c8-3a3b6615510b)
Result:
Thus the simple movement behavior was implemented successfully




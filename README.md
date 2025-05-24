# Ex5-Animator-Movement
## Aim:
To develop a animator movement for a player using unity.

## Algorithm:
## Step 1: 

Import necessary models.

## Step 2: 

 Right-click -> Create -> Animator Controller.

## Step 3: 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4: 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5: 

Drag Animator Controller to the GameObject in the Inspector.

## Program:


## PlayerController:
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float inputX;
    public float inputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        inputX = Input.GetAxis("Horizontal");
        animator.SetFloat("inputX", inputX);
        inputY = Input.GetAxis("Vertical");
        animator.SetFloat("inputY", inputY);
    }
}
```
## Output:
![Screenshot 2025-05-24 152346](https://github.com/user-attachments/assets/bd3fc169-1500-46af-933b-cd666e947876)
![Screenshot 2025-05-24 152412](https://github.com/user-attachments/assets/90358bc9-cce7-4202-bc63-ea4611a70b40)
![Screenshot 2025-05-24 152440](https://github.com/user-attachments/assets/ee3a300e-a8d3-457f-94f4-b90ccba446f9)

## Result:

An animator movement for a player using unity is developed successfully.

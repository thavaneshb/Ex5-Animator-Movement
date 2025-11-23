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

```c#
using UnityEngine;

public class movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;

    // Start is called once before the first execution of Update after the MonoBehaviour is created
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();
        
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputX", InputX);
        animator.SetFloat("InputY", InputY);
    }
}

```
## Output:

<img width="1919" height="1197" alt="image" src="https://github.com/user-attachments/assets/fa7792a3-12e3-40e1-8eb7-dfdc55f009e4" />




## Result:

An animator movement for a player using unity is developed successfully.



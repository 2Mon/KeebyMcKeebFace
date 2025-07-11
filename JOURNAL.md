---
title: "KeebyMcKeebFace"
author: "1Mon"
description: "60% Keyboard with macro keys"
created_at: "2025-7-7"
---

**Total Time Spent: 13h**

# Layout Design
I started off this project by designing the layout. Its basically a 60% layout, as my intent with this keyboard is to keep it very usable but also compact. I used keyboard-layout-editor.com to designt the layout, working mostly off the basic 60% layout. I think that this layout should be a good balance between the massive 100% keyboards and the tiny split keyboards, as it has most of the common keys without having random useless keys. Im using MX switches from Akko for this build, as they are a good budget option, with great sound and feel. 


<img src="https://github.com/user-attachments/assets/1ff742fd-78af-4883-8b52-09e767d4ab8e" width="400"/>


In this image you can see the general layout. Ideally I want to be able to put the MCU in the top right corner behind the keys, but this may not be possible. Im planning to use a Nice!Nano MCU, which has 18 pins, giving me 91 keys possible with a standard matrix. This should be plenty, as the layout I'm using is only 61 keys. This MCU also has bluetooth and a battery charging circuit, allowing me to make this keyboard wireless. 

**Time spent: 2h**

---


# Matrix + Schematic + Arrangement

In this session I designed the matrix for this keyboard. It uses an 14x5 matrix for simplicity, as if I went smaller it would be much more annoying to route. Recreating this matrix in KiCad was very annoying, as issues with the schematic and layout led to issues down the line that I needed to painstakingly fix. Here is an image of the basic matrix im using. Ill be using this as a reference for the PCB design as well as the firmware. 

![image](https://github.com/user-attachments/assets/ff8da982-1f5a-414c-af32-5c75170fb0e8)


Once I fixed some stupid mistakes, I started arranging the switches. I used a plugin that takes the layout from keyboard-layout-editor.com and the schematic and lays it out properly. This was a huge time saver, as manually arranging all the keys would have been very annoying. Ive attatched an image of the schematic for the keyboard. This inclues the keys and a connector for the battery. Im pretty happy with how clean the schematic looks. 

![image](https://github.com/user-attachments/assets/629f2811-ce4b-49f4-b103-ed2b4a524487)

And here is the layout in the PCB editor. I connected the rows and columns already, and started connecting them to the MCU. Im trying to keep it very simple, using the minimum amount of VIAs and complex connections. 

**Time Spent: 6h**

# Routing

In this session I completed the routing of the PCB. Im pretty happy with how it came out! I especially like this part, which is wiring all the columns to the Nice!Nano. I tried to use the fewest vias possible, and currnely its sitting at four on the whole board. I still need to round the corners and add a ground plane, but so far this is going very well. Ive attatched an image of the collumn connection and a full schematic image. 

![image](https://github.com/user-attachments/assets/295db0ed-8505-4fc4-94e9-149af4b3c99d)

^ This is the nicest thing ive ever made in kicad

![image](https://github.com/user-attachments/assets/66762d78-79a3-41d2-8126-7921bd7e0b07)

Full routed board!

**Time Spent: 3h**

# Final Touches on PCB

I added the rounded corners and the groundfill in this session. I had to make the edgecuts a bit larger to allow for the mounting holes, but overall its still pretty compact. Im not sure if I have enough mounting holes, so Im going to get some feedback from the community about it. Overall the PCB looks really nice and Im super proud of it. Im going to make the case next, and Ill try to make a prototype of everything to make sure it fit. Im not using a ground plane, just a normal copper fill that isnt connected to anything, as I wont be using much ground on the PCB. I routed the battery connector, a JST XH 2 pin, to the Nice!Nano as well, which should go into the rest of the board and get charged through the USB C. Im not sure which size battery I want yet, but Im planning something fairly large so the battery life is good. 

![image](https://github.com/user-attachments/assets/82e4449b-c989-4cbb-8e82-5f019e8ab71a)

Heres what the PCB looks like with the ground plane added. I will need to change around some silkscreen stuff (as well as adding some fun art) but it shouldnt change much from here. Im really happy with how clean this is!

**Time Spent: 2h**

# Beginning The Case

In this session I started designing the case for the keyboard. Im doing a sandwich mount, which means that the plate is sandwiched between the top and bottom of the plate. It also has some screws going through it so it should be very secure. The main body is currently very simple, but I plan to make it more fun with some angles and decorative bits. I might use my multi color printer to add a fun design to it, but that will be more expensive. I feel like its very boring right now. I still need to add a cutout for the USB C port and the slot for the battery, but that shouldnt take too long. 

<img width="954" height="241" alt="image" src="https://github.com/user-attachments/assets/a5ff1dba-c079-451a-a5c5-69c62f4410f0" />

Heres the sandwich mount. Basically the plate is squished between the top of the frame and the bottom of the frame. I still need to add some mounting spots at the bottom of the case to mount the PCB to, as the sandwich alone wont be rigid enough. This mounting style is very nice, as its simple and allows for a lot of customizability in the plate and case.

<img width="1209" height="663" alt="image" src="https://github.com/user-attachments/assets/25607245-4e1a-4990-80f3-052fd76b7419" />

This is the full case so far. As you can see, its pretty boring. Im going to spend a majority of the rest of my time on this project making this nicer.




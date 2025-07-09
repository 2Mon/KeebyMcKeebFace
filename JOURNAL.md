---
title: "KeebyMcKeebFace"
author: "1Mon"
description: "60% Keyboard with macro keys"
created_at: "2025-7-7"
---

**Total Time Spent: 8h**

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

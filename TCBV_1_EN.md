# TCBV

(Textbook of Changing Ballance by Virtools)

## Foreword

TCBV can be understood as a set of textbooks, which could teach Ballance players to change Ballance maps or configurations by Virtools. TCBV based on wide knowledge of using Virtools and appropriate distribution, is suitable for cartographers at different stages. You could understand Ballance mapping after learning this textbook.

## Relevant People

Written by:
* GE Fang 
* BallanceBug

Based on tutorials by:
* Nice Melodies
* jxpxxzj
* Chris Xiong

Translated by:
* BallanceBug
* GE Fang
* Tad William

*(Translations may not be 100% accurate!)*

## Content

* [Registration in Virtools](#1)
* [User Interface](#2)
* [Importing/Exporting the Map File](#3)
* [Some Basic Operations](#4)
* [Camera View](#5)
* [A Brief Summary of Objects](#6)
* [Sending Objects to Groups](#7)
* [Exchanging the Sector Groups](#8)
* [A Brief Summary of Meshes](#9)
* [Materials and Textures](#10)
* [Importing/Exporting the Source File](#11)
* [An Introduction of Lights](#12)

<h2 id="1">Registration in Virtools</h2>

Of all the versions of Virtools™ that are currently available, only two versions, 3.0 and 3.5, can be used to edit ballance maps. So please check you version first. 

A file named “devr.exe” can be found in the folder that virtools is installed. You need to register when you open virtools for the first time. (But if you cannot start it, please change the compatibility of it to **Windows XP (Service Pack 3) in settings, and run it as an administrator)**

Two options can be found when you are registering. Choose the second option **“specify the licence file”** , click “next”, then select the license file. The license file is included in the folder in which virtools is installed. After that, click “Next”, and the registration is finished. 

<h2 id="2">User Interface</h2>

When you want to learn about editing the maps in Ballance by using Virtools, the first thing you need to get used to is the user interface of virtools. We'll use the interface of Virtools 3.0 as an example to analyze for you. (And we'll abbreviate “Virtools” to “VT” in later chapters)

![assets/en_2_1.png](assets/en_2_1.png)

The frame of 3D Layout might be too small to use when you first open Virtools, so let's drag the border on the right and bottom of it to make it larger and easier to use. There are lots of objects in Level Manager, and Building Blocks on the right is almost useless for mapping, so to make it more easier, you can drag the frame of Level Manager to upper right corner, and below is what we'll see after that:

![assets/en_2_2.png](assets/en_2_2.png)

<h2 id="3">Importing/Exporting the Map File</h2>

It's obvious that the format of map files in Ballance is NMO, but the “Load” option only allows you to open CMO files. NMO files can also be loaded, but only as a source file to be imported. 

![assets/en_3_1.png](assets/en_3_1.png)

In fact, NMO map files of Ballance is actually CMO files that pretend to be NMO files. (further research shows that, as CMO supports not only map files but also animations, NMO files are the best format for static objects to be storaged) But, changing the extension name to CMO can bring you a lot of advantages. Thus it's recommended to edit and save your file as the CMO format, and change it only when you need to load it in the game.

![assets/en_3_2.png](assets/en_3_2.png)

There are three ways to save files as CMO format: Save Composition, Save As…, and Save Version. Save Composition saves the file by replacing the original file which you loaded. Save As... allows you to save the file as another names.

But, the Save Version option is rather special. It saves the file as a different name, therefore the original file will not be replaced. 

For instance, if you loaded a file named “2HAD.cmo” and edited it, using Save Version can save you a file named “2HAD_01.cmo”, but the original file is left unsaved, as the image below shows: 

![assets/en_3_3.png](assets/en_3_3.png)

Map files can also be exported directly as the NMO format. This requires you to right click on “Level” in Level Manager, and click “Save As…”, as this image shows: 

![assets/en_3_4.png](assets/en_3_4.png)

Sometimes we'll encounter another kind of NMO files, which contain only a few objects. These files are neither map files nor special configuration files. These are called sources, which are useful for mapping. To import sources to your map, the method in paragraph 1 in this chapter should be used. But it's a bit difficult to learn about importing/exporting source files, therefore, it won't be talked about in details until the next textbook.

<h2 id="4">Some Basic Operations</h2>

We will use the changed interface on section 2 to introduce the details of this section. There exists an inconvenient detail that you need to adjust the same interface every time when opening Virtools. However, it doesn’t matter mapping, we adjust interface for the convenience. Let’s see the interface which has imported a map:

![assets/en_4_1.png](assets/en_4_1.png)

Emmm … why is it nothing at all! But it isn’t a mistake. When opening Virtools every time, your location will be set to the center of the virtual world in 3D Layout. However, not all the maps are located in the center. To find objects, you need to have a series of location-change operations. The icons on the left could be understood as a toolbar. Let’s analyze the use of some common icons.

![assets/en_4_2.png](assets/en_4_2.png)

The following is a detailed description of some icons:

![assets/en_4_3.png](assets/en_4_3.png) : When selecting this icon, you could expand or shrink the view of 3D Layout by holding down the mouse. Generally speaking, you could find objects soon by this tool when editing unknown maps.

![assets/en_4_4.png](assets/en_4_4.png) and ![assets/en_4_5.png](assets/en_4_5.png) ： If you feel the default gridding is annoying, you could click them to show or hide the gridding of Virtools.

![assets/en_4_6.png](assets/en_4_6.png) : Coordinates. it represents the three vertical directions in the virtual space, so it is the basis of object-locating. 

![assets/en_4_7.png](assets/en_4_7.png) : When selecting this icon, you could move the viewport by dragging your mouse.

![assets/en_4_8.png](assets/en_4_8.png) : Adjust View by Revolving around Objects: When nothing is selected, you could revolve the viewport around the center of the virtual world. Therefore you need to select something at the center of the view at first to prevent the camera from running wild. You could select one or several objects and drag the mouse, then, the camera will surround your selection. Try holding down ![assets/en_4_9.png](assets/en_4_9.png) , and you will see three selections: ![assets/en_4_10.png](assets/en_4_10.png) Drag the mouse on ![assets/en_4_11.png](assets/en_4_11.png) and loosen, ![assets/en_4_12.png](assets/en_4_12.png)  become ![assets/en_4_13.png](assets/en_4_13.png) . Then you could use it to rotate the camera’s direction directly.

![assets/en_4_14.png](assets/en_4_14.png) : Forward and Backward Moving: Like ![assets/en_4_3.png](assets/en_4_3.png), but if you holding down the mouse and change it to ![assets/en_4_15.png](assets/en_4_15.png) , when you click it, the view will be moved to just enough space for the selected object(s) after selecting object(s) and click. (We'll learn how to select objects next). This tool is useful.

![assets/en_4_16.png](assets/en_4_16.png) : Select Object(s): Click to select one object and drag mouse to select all objects in the selected area. You could hold down the key ”Ctrl” and click objects to select several specified objects. 

You should keep the mouse on the selected object(s) to use object-operating tools, if not, it will break your selection, sometimes lead to some wrong operations. It's suggested you click ![assets/en_4_17.png](assets/en_4_17.png) to lock your selection, and you could click any place in 3D Layout to operate on selected object(s).

By the way, when you want to drag the mouse to select objects, you need to understand the following things:

![assets/en_4_18.png](assets/en_4_18.png) means that the selection box can select any object which is in a part of the selection box, so this can cause mistakes easily. Therefore, it's suggested you click it and change it to ![assets/en_4_19.png](assets/en_4_19.png) . Then, only the object(s) completely in the selection box can be selected. You could click ![assets/en_4_20.png](assets/en_4_20.png) after selection to check if there exists a mistake choice.

![assets/en_4_21.png](assets/en_4_21.png) : Moving Object(s): After selecting object(s), you could select a coordinate or a plane composed with two coordinates. Then you could move selected object(s) based on the selected coordinate or flat. Such as the following picture, after selecting flat Z+X, you can only move selected object(s) on the plane Z+X, and the objects cannot be moved on coordinate Y.

![assets/en_4_22.png](assets/en_4_22.png)

![assets/en_4_23.png](assets/en_4_23.png) : Rotating Object(s): Like moving object(s), You could select one or two axes to rotate. However, it is a bit difficult to determine. In fact, object(s) rotating is not commonly used, later, we will learn how to rotate an object accurately by adjusting the object setup. 

![assets/en_4_24.png](assets/en_4_24.png) : Expanding or Shrinking Object(s). This tool is not commonly used in Ballance mapping, and using it may cause some problems. 

![assets/en_4_25.png](assets/en_4_25.png) : Place a point light (like a light bulb) in front of the view. You could use it to light the map. After all, point lights aren’t the inherent things in the original maps, and a map included point lights may cause some bad-visual influence. Therefore, you should delete point lights after mapping. (The point light is only one kind of lights, we will learn more about lights in the future) 

<h2 id="5">Camera View</h2>

We have learnt a number of the operating icons. The other icons have little influence on Ballance mapping, so we don’t have an introduction of them. If you are interested in them, you could explore them by yourself.

You could learn how to adjust the camera view in this section. You could select camera mode by right-click the 3D Layout. You could also find the mode” * View” on the 3D Layout and click to select the camera mode. It’s shown in the picture below:

![assets/en_5_1.png](assets/en_5_1.png)

You could have different operations with different view. The following is an introduction to them.  

The default view is Perspective View, which is the most common view of maps. There exists a vanishing point in Perspective View, so Perspective View could reflect the rule about far-small and near-large. Therefore, if we are in the scene, we could see the effect of Perspective View. Perspective View is also used in art.  

Top View, Front View and Right View are all projected from one direction. With them, we can also accurately move the object(s) based on a specified plane or a specified coordinate axis.

---
Still waiting to be translated ...

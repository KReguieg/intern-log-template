# 🚀🚀🚀My Internship Log🚀🚀🚀

This document is my personal log. It shows/documents my journey with the immersive insiders team and my personal development.

Most important is not a lot of text, but very concentrated text that explains the **essence** of what I did/tried/learned/discovered!!!

## Week 1 2021-03-01

### ✅My Tasks
- Create/search a phone/scanning image
    - Create a animation from it in Unity
- Learning about branching and git flow
- Solid Principles   

### 📚What I learned
- There is this website [TheNounProject](https://thenounproject.com/)
    - it offers a whole world of nice high quality icons
    - I should keep in mind to credit the author otherwise it is "stealing"

- Git
    - Git Workflow
        -  Use 'git status' to check for current status of files - it will highlight the modified files in red.
        - Use 'git add' to add the files which have to committed and pushed, add only the files that were edited.
        - Use 'git commit -m "some text" ' to commit your changes, before committing make sure to add a short note using -m " " ,note should mention what modification one has made
        - Use 'git push' to finally push it to your repo in the server.
    - If credentials of a git user already exit , it can be easily changed by 
        - Type  " git config --global --user " . Which will open the following screen
        ![](img/Git_Config_snipping.JPG) 
        - At the bottom you can see the path at which the config file is located 
        - Navigate to that path, open the file and enter your git email.
        - Whola ! it's done !

- Blender [Need to work on this in the future after getting my VR headset]
    - We can render blender models into VR Devices directly to see the preview.
    - Following are the simple steps as to how that feature can be enabled
        1. Edit -> Preferences -> Add-ons
        2. Search for VR and ☑ check the box for "3D View: VR Scene Inspection"
        3. In 3D View , select View tab and choose your VR Camera
        4. In 3D View , select VR tab and click on Start VR Session
        
        ![](Vid/Blender-VR.gif) 


- Unity Programming
    - Learnt to use Invoke function 
        - I wanted to delay the start of my game by few seconds, I thought I could use coroutines and make the function to wait for few seconds, but that logic does not work , because in coroutines the function is already executed , it returns void.
        - After some researching I found out about *Invoke* Function, using this you can invoke a function after a certain time duration. This solved my problem. 
        - Syntax : Invoke("Function_name_in_form_of_staring", delay_duration)
    

- Programming Principles 
    - Learnt the S O L I D , principles 

### 🛠Created
- Tried with this image 
 ![](img/HandPhone.png)

    *author: Hand Phone by Jonathan Wnty from the Noun Project*


- But since my game required to hold the phone with both hands, I changed it to the below image ![](img/holding_smartphone.png)

*author: hands holding smartphone by Atif Arshad from the Noun Project*

This is how it looks after animation: 

![](Vid/MobileAnimation.gif) 

Version 2 :

![](Vid/MobileAnimationv2.gif) 

-------------------------------------

## Week 2 2021-03-08

**USE BRANCHING FOR WEEK 2!!! create a branch which is named log-update/week-2**...

...and add your changes for week two in it, next monday we are going to review the branch and merge it into main"

### ✅My Tasks
 - Learning about branching and git flow
- Solid Principles   

### 📚What I learned
- Formatting text in TextMesh Pro
    - For my game I had the credits canvas and I wanted  it to look clean and neat.
    - Initially I tried formatting it in a word document and pasting it in the unity's text box, But realized that it does not work that way!
    - After looking up for it in google I found this website :
    [Digital Native Studios](http://digitalnativestudios.com/textmeshpro/docs/)
    - It has documented all the different type of formatting that can be done using TextMesh Pro.
    - I learnt to use the tags, they were similar to a HTML tags.
    - I learnt how to download sprite sheet, use the sprite editor to split it and use the tags in TextMesh pro to display the sprite as emojis.
    ![](img/Sprite-Atlas.PNG)
    - Basically to represent the words "VISUAL" and "MUSIC" as icons, highlighted in yellow box below.
    ![](img/TextMeshPro_emoji.PNG)
    -  And what you see below is me using those features to modify the text as per my requirement.
        ![](Vid/CreditCanvas.gif) 

- Git 
    - Learnt how branching is done, below is the correct flow of commands that has to be followed.
        - Check for status, add the edited files , commit and push to your main i.e the forked repository also called as origin 
        - Go to git hub and Merge the pull request from the upstream.
        - Now the upstream content will be merged to your main 
        - Pull this main into your local drive.
        - Create a branch for this using the command "git branch log-update/week-2"  
        -Now that your branching is complete in your local and to see the same in you github, you can check for status, it will show which branch you are in and then if there is nothing to commit proceed to push it.
        - Now that we have a branch ,to push it its always a good practice to mention the path where it has to be pushed to,so for my case the command looks like : git push origin log-update/week-2

- Blender
    - Learnt how to add textures and material to 3D models.
    - I attempted to add the material and textures, but when i exported it and imported it in unity the textures were missing.
    ![](img/blender_texture.PNG) 
    ![](img/blender_texture2.PNG)  
    - So need learn as to how a model should be correctly exported to unity.

- Unity
    - Optimization is important and today I learnt that the texture take up a lot of memory.
    - The size that shows up in your file explorer is the physical texture size and the size that shows up in unity editor is the Game memory size.
     ![](img/imgsize.png) 
     
     - If you want to save up the memory while the game is running you can decrease the max size in the editor
     ![](Vid/Texture_Size_reduction.gif) 
     - I ended up saving a lot of memory 💾. As you can see above just by halving the size , the memory is reduced by 10X.  

### 🛠Created

- Created Virus model with different texture:
![](Vid/virus_texture.gif) 


- As the texture was not imported from blender, the actual creation happened in unity editor editor this is how it looks: 

![](Vid/Virus_newtexture1.gif) 
![](Vid/Virus_newtexture2.gif) 

- Sadly they did not look that good when Augmented:

    ![](Vid/Virus_AR1.gif)
    
    ![](Vid/Virus_AR2.gif)

## Create github.io website from the log

- I have created my github.io but its not yet ready, I am yet to learn how to edit it and make it look good.
 - Here is the link :https://ashraypai.github.io/intern-log-template/
    

## Week 3 2021-03-15

### ✅My Tasks
- Helping With VR course
- Unity Design Principles
- Learning about particle effects in Unity  

### 📚What I learned
- Creating Augmented Reality Inside of Virtual Reality
    - We were able to create a model of tablet with camera and that would be able to use Ray-cast to detect images and spawn 3D objects.
    - The 3D model then could be pulled into VR by using events and changing the events

- Learnt to use the VFX graph in unity to  create cool Particle effects.
    - Used the VFX graph to create the Fireworks with Immersive insider logo.
    - I referred to this video :https://www.youtube.com/watch?v=iCEHarLRCzI to create the basic rockets.
    - And then refer to this video : https://www.youtube.com/watch?v=r2Eoy3-p-xc&t=541s to create the 2D images as particle effects.

- Learnt to create 3D models in Blender
    - Used the add on from https://keentools.io/ 
    - Referred to the tutorials on their website and this video : https://www.youtube.com/watch?v=5WH7s-IPIeM to model my face in blender.

### 🛠Created

- Fireworks using particle effects and VFX Graph
    ![](Vid/Fireworks.gif)

- 3D model of my face , ( Yes! does not look like me, definitely needs improvement)
     ![](Vid/Blender_face_2d.gif)

     ![](Vid/Blender_face_3Dmodel.gif)

- Created Particle Effects out of that 3D model
    ![](Vid/FaceModelEffect.gif)


## Week 4 2021-03-22

### ✅My Tasks
- Unity Design Patterns  
- Blog on AR Setup   
- Blog on Creating Fireworks effect using VFX Graph and Post Processing

### 📚What I learned
- Learnt the following Unity patterns :
    - Singleton
    - Object Pooling
    - Observer 
    - Component 
    - Flyweight
![](img/UnityDesignPattern.png) 

### 🛠Created

- The Blog on AR setup here in this link : https://github.com/ashraypai/BlogPosts/tree/master/AR%20Setup

- The Blog on VFX graph and PostProcessing can be found here in this link : https://github.com/ashraypai/BlogPosts/tree/master/VFX%20Graph

## Week 5 2021-03-29

### ✅My Tasks
- C# intermediate concepts 
- Blog on VR setup and XR Simulator Controls
- Snapchat Lens


### 📚What I learned
- Learnt the following concepts in C# :
    - Interface ✔
    - Inheritance ✔
    - Polymorphism 
    - Delegates 
    - Lamda expressions

![](img/C_Concepts_1.png) 

- Learnt to use the Lens Studio software from Snpachat, to create AR lens.This software has accurate face, hand and body tracking. 
I have created 2 lens, to try it, open snapchat and scan the below code
    1. Immersive Trial :

        ![](img/Immersive_trial.png)
    
    2. Immersive Cap:

        ![](img/Immersive_cap.png)

### 🛠Created

- The Blog on AR setup here in this link : https://github.com/ashraypai/BlogPosts/tree/master/AR%20Setup

- The Blog on VFX graph and PostProcessing can be found here in this link : https://github.com/ashraypai/BlogPosts/tree/master/VFX%20Graph

- Created Immersive Insider lens 

    1. Immersive Trail:

        ![](vid/Immersive_trial.gif)

    2. Immersive Cap:

        ![](vid/Immersive_cap.gif)

# AnimRec_Utilities
Tools for the VRChat world "AnimRecStudio".

"AnimRecStudio" is a world in VRChat where you can capture movements and generate animation clips.  
You can create animation clips using the tools distributed here.  
![worldthmb](https://github.com/user-attachments/assets/ca30a860-832b-4ec6-ad10-59a0a7fc6494)

## Json2Anim Converter
Receives data from the VRChat client and converts rotation information into JSON human skeleton data.
### How to use
#### Step 1
Start Json2Anim.exe and make sure that "Monitoring client log file..." appears on the screen.  
**Warning: Make sure that debug log output is enabled in the VRChat settings.**
![json2anim_page0](https://github.com/user-attachments/assets/5dd85222-29b5-486f-99a8-3d07f5a971e5)
#### Step 2
After exporting the file to the log on the AnimRecStudio side, return to Json2Anim.  
Confirm that the animation preview screen is displayed as shown here.  
You can check the recorded animation by pressing the play button.  
![json2anim_page1](https://github.com/user-attachments/assets/bb1c79e5-d439-46c6-8129-e3a76fd7856e)
#### Step 3
Once you click the "Export" button, the "Processing" window and a progress bar will appear.  
This may take some time for long animations.  
![json2anim_page2](https://github.com/user-attachments/assets/6e79b57e-4f2e-4978-a768-c551429df493)
#### Step 4
Once processing is complete, a window will appear allowing you to select a save destination.  
Select a save destination and click "OK" to save the JSON file.  
This completes the process.  
See the next section for information on converting to an Anim file.  
![json2anim_page3](https://github.com/user-attachments/assets/867be11b-06cd-4c6e-8c89-152dad96c873)

## JsonAnimImporter
Generates a humanoid animation file based on Unity human muscle data converted by Json2Anim.
### How to use
#### Step 1
Import the unitypackage distributed here into your avatar project.  
After the import is complete, make sure that 
the "TaaDev" item is present in the menu bar.  
**Warning: Do not move the JsonAnimImporter directory!**
![jsonanim_page0](https://github.com/user-attachments/assets/f0537021-b84d-4bc4-b2ec-e081ddf12468)
### Step 2
Launch the importer from "TaaDev/Anim Importer" on the menu bar.
Click "Select file & Import clip" and select the corresponding JSON to generate an animation clip,  
then select the destination to save the anim file and create and import the file.  
Setting the keyframe reduction option can reduce the upload size of the avatar (but movements will become unnatural).  
![jsonanim_page1](https://github.com/user-attachments/assets/1fd1e135-75ab-4daf-9f21-19b79915181c)

# Face-Swapping
### Project Goal
The goal of this project is to make a snapchat filter. This filter will find your face and replace it with any image you choose, if you decide to use a different image than the one provided to you either change the file name to 'cartoon.jpg'(like you see in this github folder) or go into the code and add your file name there. When you run the .ipynb a new .avi file will be created in the folder containing the ipynb called "output.avi", this avi file is just a recording of the filter and starts as soon as you run the code. If you run the code you should know pressing the 'q' key on your keyboard will end the code. Upon running the ipynb file, you will see 2 windows pop up. One of them will be a small window that will only show you your face along with blue circles to show you the location of your eyes. The other window will have 2 live feeds from your camera, the one on the left will show your face with a green bounding box and blue circles for your eyes. The one on the right will show you with the cartoon filter applied to it.  

### Process
  
  - get and initialize Opencv's face and eyes classifier
  - import cartoon image: `cartoon = cv2.imread("cartoon.jpg")`
     - if you plan to import your own image 
         - please make sure the image is in the same folder as the ipynb file
         - change "catroon.jpg" with then name of your image file in quotes    
  - Turn your camera on
  - Set parameters for recording filter
  - capture each frame of the video and grayscale them
  - find faces and eyes for each face
  - reshape the image to fit over face
  - keep image on face
  - display all windows/frames
  - check for wait key to break for loop
  - deactivate camera and close all windows

### Result
The results were very good as the tracking was better than I expected. I plan to learn how to make a bounding box that covers exactly the face rather than a rectangular bounding box. This way the filters will look more professional.

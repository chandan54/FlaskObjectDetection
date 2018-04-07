# Assignment_DataPeace
//Steps to run the object detection framework deployed using MobileNet SSD pretrained model and Postman REST API.
#Steps to run Postman.
    REFER: https://www.getpostman.com/docs/v6/


1. For images available on localhost (i.e. Images are in the same folder in which the app_flask.py exists or if the image is not in the same folder give the full path to the image  )
    POST {"image_path":"image.jpg"}
    (Here image.jpg is the name of the image and the above command has been run on Postman)
    
    
    
2. For images available online(i.e.User has the access to the image address/link) 
open the app_flask.py and uncomment the lines 26 to 32 and save the app_flask.py file and replace image_path with temp_file in the below command.
    i.e. Line no:33 in app_flask.py
    image = cv2.imread(image_path) with image=cv2.imread(temp_file)
Once saved, open Postman and  execute as 
    POST{"image_path":"image_link"} 
    //for example POST{"image_path":"https://thumbs.dreamstime.com/b/cat-dog-beach-chair-sitting-blue-white-deck-95561167.jpg"}
    
Video of implementation:
# https://drive.google.com/file/d/11VzHou9SNok-XVSZMmU41mbDgMvWAa_g/view?usp=drivesdk

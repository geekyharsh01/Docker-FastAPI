This repository Contains the dockerfile which includes the code to build a docker image that can be used to open the python fastAPI app created previously.
Find the link of the Python Project FastAPI - https://github.com/geekyharsh01/Python_Project
How to run the dockerfile and then finally run the FastAPI app:
step1- Download this repository as well as the Python_Project repository link is provided above.
Step2- Extract the dockerfile in any one folder and then copy Python_project folder into the same directory.
       The Directory Structure should look like :  --Parent_folder -- dockerfile (and other docker related files)
                                                                 |--- Python_Project -- api(folder) and other files

Step3- If you have'nt installed Docker Desktop then install it and then run it.
Step4- open terminal in the directory where dockerfile is present and type the command -  " docker build -t yourImageName .  "
       Don't forget to put dot at end as it is shown in the command, after running this command , It will take some time to build the image for you.

      After creating the image , you can type "docker images"  to see the your built image of this application.

Step5- Go to the Docker Desktop and in the images you can see your built image with name yourImageName , Now Run that image and in the optional settings 
      Put 8000 or any other suitable port you like and then Run the image , It will create a container and the program inside it will start running.

Step6- Access your web Appilcation by clicking on the 8000:8000  this kind of link shown in the docker Desktop at the top of the log which you see when the container is running.
       or you can access at localhost:yourport , yourport is the port number you gave earlier while running the image in the optional settings.

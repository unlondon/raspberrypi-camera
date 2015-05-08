# raspberrypi-camera
Python code for the raspberry pi camera

https://www.raspberrypi.org/learning/python-picamera-setup/worksheet.md

https://www.raspberrypi.org/documentation/usage/camera/python/README.md

Install the camerea library

##sudo apt-get update
##sudo apt-get install python-picamera

First, at the Python prompt or at the top of a Python script, enter:

    import picamera
    
This will make the library available to the script. Now create an instance of the PiCamera class:

    camera = picamera.PiCamera()
    
And take a picture:

    camera.capture('image.jpg')
    
HORIZONTAL AND VERTICAL FLIP
Like with the raspistill command, you can apply a horizontal and vertical flip if your camera is positioned upside-down. This is done by changing the hflip and vflip properties directly:

    camera.hflip = True
    camera.vflip = True
    

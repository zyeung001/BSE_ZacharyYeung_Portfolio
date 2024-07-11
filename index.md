# Ball Tracking Robot
<!-- Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails! 
-->

The ball tracking robot uses object tracking to follow the ball. With the use of the Python Library, OpenCV, the camera can recognize faces, detect objects, and much more. This project uses a Raspberry Pi, Pi Camera, Motor Driver to control the motors, DC Motors to control the wheels, and a Ultrasonic Sensor to avoid object collision.


<!-- You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:-->
  
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->


| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Zachary Yeung | Lynbrook High School | Engineering | Incoming Sophmore

<img src="Zachary_Y.JPG" alt="Zachary Yeung Headshot" style="width:536px;height:736px;">



<!--
# FInal Milestone
For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE
-->

# Third Milestone


<iframe width="560" height="315" src="https://www.youtube.com/embed/aX1jdvUm-GE?si=vX5lI-Bp5G8XKcDt" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Summary
For my third milestone, I incorporated the ultrasonic sensor into my project. When the robot gets to a certain distance from an object, it will stop moving until the object moves further away. 

## Challenges
I wanted to utilize the two other ultrasonic sensors in my project, but when I used three ultrasonic sensors, the frames for my PiCamera dropped from 60 fps to around 3 fps. This made it pretty hard for my robot to track the ball, so I only used one. I tried using threading which is running multiple functions or codes at the same time. This method succeeded in keeping the fps at 60, however I realized I will have to cover the right and left ultrasonic sensor for my modification. 

## What's Next?
I plan on adding a way for the robot to take the ball and bring it back to me by using servos to take the ball and implementing odometry using wheel encoders.


# Second Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/p5iCH_pKMqY?si=aI6CMq3StmQI1W9M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Summary
My second milestone is to code the ball tracking for my robot. The main components I used for the second milestone is the Raspberry Pi, PiCamera, and the motors. The code I wrote first creates a contour around the ball with x and y as the center of the contour. The x value is the width of the frame. Based on this, if the x value is on the right side of the frame, then the car moves to the right. If the x value is on the left side of the frame, then the car moves left. If the ball is around the middle of the frame, the car moves forward. Lastly, when no contours are detected, the car will turn constantly turn right until it finds anything red.

## Challenges 
A challenge I faced was coding because I didn't really know how to code. So I used many different tutorials to create my ball tracking code. Another challenge I had was when I finished coding the ball tracking, the car would only move left and right to get to the ball, which was fixed when I added a middle range where it could move forward. The last challenge I had was setting up VNC so that I could run the Raspberry Pi without connecting it to my laptop. It only worked once for me, but now it never works.

## What's Next?
For the next milestone I am going to use the ultrasonic sensors to avoid colliding into object. I also might try to set up the VNC again.


# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/iaNKyVHkxec?si=Xjp5Ty7hhWd-078Z" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Summary
My first milestone is wiring up all the components of the robot and making sure that it work. The components I used are the Raspberry Pi, DC motors, a motor driver, ultrasonic sensors, and a PiCamera. The Raspberry Pi controls all the components, the DC motors spin in certain directions, the motor driver amplifies current to the DC motors, the ultrasonic sensors calculates distance, and the PiCamera is a camera. Right now, the motors spin, the PiCamera works fine, and the ultrasonic sensors work. Later on I will write code so that it will track a ball using the PiCamera and if the ball moves, the robot will follow it. I will also use the ultrasonic sensors to avoid crashing into obstacles like the ball. 

## Challenges
One challenge I faced during the first milestone was setting up the Raspberry Pi. I was confused because not only did you have to set up the MicroSD card but you also had to download certain softwares to display the Raspberry Pi on a device. I also had a hard time setting up the SSH for the Raspberry Pi, which is a way to connect the command promt on your computer to the Raspberry Pi terminal. Everytime I tried connecting to the Raspberry Pi through SSH, it would say that it cannot find the Raspberry Pi. 

## What's Next?
For the next milestone, I will code ball tracking, and making sure that the robot follows if the ball moves.


# Starter Project

## Summary
For my starter project, I created the game console. I chose this project because it seemed coolest out of all the starter projects. This game console includes Tetris, Snake, Racing, Space Invaders, and Slots. How this game console works is whenever a button is pressed, it sends a signal to the chip, which is then displayed on the LED dot matrix. The red switch is used to turn on the console, the yellow button is used pause the game, the green button starts the game, and the blue buttons controls the LEDs. 

## Challenges
A challenge when creating this starter project is soldering. I accidentally burnt some parts with the soldering iron, but my game console still works. To avoid this, pay attention to what your soldering iron is touching. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/jPP67IPjiLI?si=dl3Rb8Yc3AZLC_-7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<!-- # Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 
-->

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```
import RPi.GPIO as GPIO
import time
import cv2
from picamera2 import Picamera2
import numpy as np
from gpiozero import Servo

GPIO.setwarnings(False)



# To use Broadcom GPIO numbers instead of using board pi numbers
GPIO.setmode(GPIO.BCM)


servo_right = Servo(16)
servo_left = Servo(12)

servo_right.detach()
servo_left.detach()

in1,in2,in3,in4 = 2,3,17,27


TRIG_FRONT = 23
ECHO_FRONT = 24
# Front Sensor
GPIO.setup(TRIG_FRONT, GPIO.OUT)
GPIO.setup(ECHO_FRONT, GPIO.IN)
# Set the trig pin to low
GPIO.output(TRIG_FRONT,False)
   

# Setup the ouput pins
GPIO.setup([in1,in2,in3,in4],GPIO.OUT)

GPIO.output([in1,in2,in3,in4],GPIO.LOW)



# Create a Picamera2 instance
picam2 = Picamera2()
# Configure camera settings (adjust as needed)
config = picam2.create_preview_configuration(main={"format": "XRGB8888", "size": (640, 100)})
picam2.configure(config)
picam2.start()


def sensor():

    # Wait 50 miliseconds and set trig to high for a new ultrasonic pulse transmission
    time.sleep(0.05)
    GPIO.output(TRIG_FRONT,True)
   
    # Set it back to low after this pulse to wait for the pulse to bounce back
    time.sleep(0.00001)
    GPIO.output(TRIG_FRONT,False)

   
    # If no pulse returns ECHO is 0 and it records the time. When there is a pulse ECHO becomes 1 and it also records the time using time.time()
    while GPIO.input(ECHO_FRONT) == 0:
        pulse_start = time.time()
    while GPIO.input(ECHO_FRONT) == 1:
        pulse_end = time.time()
   
    pulse_duration = pulse_end - pulse_start
   
    distance = (pulse_duration * 34300)/2     # distance = (time * speed of sound [34300 cm/sec]) / 2
   
    return round(distance,2)          # rounds the distance by two decimal places


def motor(x, distance):
    timer_started = False
    start_time = 0
    if distance > 5:
        if x >= 430:   # turn right
            GPIO.output(in1,GPIO.LOW)
            GPIO.output(in2,GPIO.LOW)
            GPIO.output(in3,GPIO.LOW)
            GPIO.output(in4,GPIO.HIGH)
               
        elif x <= 210:   # turn left
            GPIO.output(in1,GPIO.HIGH)
            GPIO.output(in2,GPIO.LOW)
            GPIO.output(in3,GPIO.LOW)
            GPIO.output(in4,GPIO.LOW)
           
        elif 210 < x < 430:     # move forward
            GPIO.output(in1,GPIO.HIGH)
            GPIO.output(in2,GPIO.LOW)
            GPIO.output(in3,GPIO.LOW)
            GPIO.output(in4,GPIO.HIGH)
           
        elif len(contours) == 0:
            GPIO.output(in1,GPIO.LOW)
            GPIO.output(in2,GPIO.LOW)
            GPIO.output(in3,GPIO.LOW)
            GPIO.output(in4,GPIO.HIGH)
       
  #  elif distance <5:
      # if not timer_started:
           # start_time = time.time()
          #  timer_started = True
           
    else:
        GPIO.output([in1,in2,in3,in4],GPIO.LOW)

        print("stop")
       
        servo_right.max()
        servo_left.min()
        time.sleep(1)
        servo_right.min()
        servo_left.max()
        time.sleep(1)
        servo_right.detach()
        servo_left.detach()
       

       
           
while True:
   
    # Capture a frame from the camera
    frame = picam2.capture_array()
    hsv_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2HSV)
   

    # Detect the ball (you'll need to adjust the color range)
    lower_color = np.array([150, 140, 1])
    upper_color = np.array([190, 255, 255])
    mask = cv2.inRange(hsv_frame, lower_color, upper_color)
    mask = cv2.erode(mask, None, iterations=2)
    mask = cv2.dilate(mask, None, iterations=2)

    # Find contours and track the ball
    contours, _ = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
    if contours:
        ball_center = max(contours, key=cv2.contourArea)
        ((x, y), radius) = cv2.minEnclosingCircle(ball_center)
   
        if radius > 10:
            cv2.circle(frame, (int(x), int(y)), int(radius), (0, 255, 255), 2)
           
        distance = sensor()
        print(distance)
        motor(x, distance)
       
    # Display the frame
    cv2.imshow("Ball Tracking", frame)
    key = cv2.waitKey(1) & 0xFF
    if key == ord("q"):
        break

   
# Clean up
cv2.destroyAllWindows()
picam2.stop()
GPIO.cleanup()


```

# Bill of Materials

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Canakit | Contains Raspberry Pi 4 Model B, USB-C power supply, USB MicroSD card reader, MicroSD card, Micro HDMI to HDMI Cable, USB-C PiSwitch, and a case to hold the Raspberry Pi | $119.99 | <a href="https://www.amazon.com/CanaKit-Raspberry-4GB-Starter-Kit/dp/B07V5JTMV9/ref=sr_1_4?crid=22X0E9O7J0OR7&dib=eyJ2IjoiMSJ9.4wZGiZcG7IfVeIs8ylcbr2OWb6dH50gzNdgVi5k-In6pZ99iy8liii7M868UpE97GOIE-tJXQ5sL2XcKGA1wfI3W6mEWsgK1idpK8oIafYN0mPwGntfbsrb3OPGDrrX_z_IS2KvZHiD7YuKDlCT3yoBjG8MgoEI2mzIFUcrNXi1b6c5wWa4Xqelg7oT0q23ZSCpLWxLI0gNwJZzD2KRFfstDIQSowiGKue1IxIrNLrDMGPsu5nPkHQfMaD2q6Fg0okZFAKlMpuxR8LUT6OFyvHql6sTdWpX5KHS5CKILFRI.3BQRKh7cMpx9AbLHH4-SPcHXiP2O2R9GGyI4xqScCfg&dib_tag=se&keywords=raspberry%2Bpi%2B4&qid=1718655031&s=electronics&sprefix=raspberry%2Bpi%2B4%2B%2Celectronics%2C181&sr=1-4&th=1"> Link </a> |
| 4 L298n motor drivers | Controls the DC motor | $9.99 | <a href="https://www.amazon.com/BOJACK-H-Bridge-Controller-Intelligent-Mega2560/dp/B0C5JCF5RS/ref=sr_1_4?crid=23DST39Q577P8&dib=eyJ2IjoiMSJ9.SUwZQBGEhgO-mVLMGJaDlCUDqIV_oiFZsqgrdyMhBBXjgOelzUnGWWEp_An1L0-GmkQAr2J3MIAKIjnGLYk0aHOAHd90jdDYlzI4ytEMfDW7P5UH6mIOKJl2hzLmGOUGISu2N2N7HeHcsLIXxVn0pQKMyIFfcOkBGchxHFqDqVt0C8IutcXgjigRpoTXAP6gyQedtSbWR_ZZLFf4dUfcl4sdgScCQsgaPK_B0a5ZTZw7xEUoEJPPV4ATW_vlbgYl3iC23NydA4Ebr1fR3NBXQ4s-Tdez_VsTr9nl6fkqutA.O1T7Zh-oncidOqMrf4k0FtQw-X2V4ZF7dUEo9-pAs8U&dib_tag=se&keywords=motor+driver&qid=1718661957&s=electronics&sprefix=motor+driv%2Celectronics%2C167&sr=1-4"> Link </a> |
| Robot Car Kit | Kit with a robot car chassis, DC motors, and tires | $12.99 | <a href="https://www.amazon.com/Smart-Chassis-Motors-Encoder-Battery/dp/B01LXY7CM3/ref=sr_1_4?crid=27ACD61NPNLO4&keywords=robot+car+kit&qid=1689698962&s=electronics&sprefix=robot+car+kit%2Celectronics%2C169&sr=1-4"> Link </a> |
| Ultra Sonic Sensors | 3 Ultrasonic Sensors with 3 acryllic mounts, female to female wires, and male to female wires | $7.99 | <a href="https://www.amazon.com/WWZMDiB-HC-SR04-Ultrasonic-Distance-Measuring/dp/B0B1ZZRZZH/ref=sr_1_3?crid=384W98YF7N1M8&dib=eyJ2IjoiMSJ9.qHehPV3yhLYm-WByKmLQatLayt48t7aTFzH7Zfqk2JNKommz196RtpF8hq3_cEwxvDgyqX0y7G6hQSsBc3FEmOVKReBL3CS6KTS9p62gEzfNdV8PKm5ayvJf4lYBC0FrYhRYDH47DxcOEc3-s-7dBRX4oQuVeEEEV5yFLWxBWcJgw2CSeFVv_0_NpZYrKFrh1HygGAe8TSV1Z5BuLR0-Hx09gpXeiFFj09BIW1_nnzmJV5F1ybScBwLxTXMRekdHvZEA6Ocqf7UBsIdkm5EAO26Yzdgyj0A3kic5H2TNtJw.M1hntwP-Ey7wLUMDLGuXL7A_OZov-sO0RYTrFDKOAo8&dib_tag=se&keywords=ultrasonic+sensor&qid=1718662182&s=electronics&sprefix=ultrasonic+sensor%2Celectronics%2C152&sr=1-3"> Link </a> |
| Pi Camera | Contains a Pi Camera and a acryllic case | $12.99 | <a href="https://www.amazon.com/Arducam-Megapixels-Sensor-OV5647-Raspberry/dp/B07RWCGX5K/ref=sr_1_4?crid=1PVMDEOQGH5ED&dib=eyJ2IjoiMSJ9.SdZxeeuAaWgC9GeoeEJUFOyYjAeqdEP5pZ9Cy64vaBUDFDfDopOIAuEwsDCEwVgfLaflgS0hj7mfOh0_-RyEVzDr3siS_eE8bNteSPWJzARX0hLEWEtFnnB7a6w5RW1UrZxf7UxLNd5-suSzDDenm5_SZ-xv7-owqJDvMCV4r1hjCrVfcCmkj9omLyiqXwW3QBgGRGjD6dNITf_VmFvw4NVTL45aFFzw8dg-KTjkdNayWu8JlRiTd1ShYc41rT8V8HZ_XVr5ChSygVIAw2IckrGLsrQJmdvU45VPCA2S9FY.oUjWRUtlVtW_oQuZV-BcJgIjXydxPxhkrD-Bn7IxZWY&dib_tag=se&keywords=Pi%2Bcamera&qid=1718662766&s=electronics&sprefix=pi%2Bcamer%2Celectronics%2C155&sr=1-4&th=1"> Link </a> |
| Soldering Kit | Contains a soldering iron and solder wire | $12.67 | <a href="https://www.amazon.com/Arducam-Megapixels-Sensor-OV5647-Raspberry/dp/B07RWCGX5K/ref=sr_1_4?crid=1PVMDEOQGH5ED&dib=eyJ2IjoiMSJ9.SdZxeeuAaWgC9GeoeEJUFOyYjAeqdEP5pZ9Cy64vaBUDFDfDopOIAuEwsDCEwVgfLaflgS0hj7mfOh0_-RyEVzDr3siS_eE8bNteSPWJzARX0hLEWEtFnnB7a6w5RW1UrZxf7UxLNd5-suSzDDenm5_SZ-xv7-owqJDvMCV4r1hjCrVfcCmkj9omLyiqXwW3QBgGRGjD6dNITf_VmFvw4NVTL45aFFzw8dg-KTjkdNayWu8JlRiTd1ShYc41rT8V8HZ_XVr5ChSygVIAw2IckrGLsrQJmdvU45VPCA2S9FY.oUjWRUtlVtW_oQuZV-BcJgIjXydxPxhkrD-Bn7IxZWY&dib_tag=se&keywords=Pi%2Bcamera&qid=1718662766&s=electronics&sprefix=pi%2Bcamer%2Celectronics%2C155&sr=1-4&th=1"> Link </a> |
| Logitech wireless keyboard and mouse | Wireless keyboard and mouse | $16.49 | <a href="https://www.amazon.com/Logitech-MK270-Wireless-Keyboard-Mouse/dp/B079JLY5M5/ref=sr_1_3?crid=1EB2IM5QZZM0E&dib=eyJ2IjoiMSJ9._sPvKwcMOsOmIdgxqvnWV4id3VFXF9Kq45I6Brnt4pkYHSrW5iW7niF-hFW1evu1u93ERoZx7djI2gT0ASavl-0XccE4I7eEp3tqqw3EyD5O18acWyupPhIelxTCryo18vIK3eqXAkOiWqF-glFJi3GeyJNerBxpMHb1SucHIKqG5HwgB14pO2xtnOOQO-ecC3UtvEdziACHE44qSvj8JdiNNiY41zzbou35mPzlris.5SMV4AF30xvtok3fYJbh1n0frD-lnIc2rOV0w3te61M&dib_tag=se&keywords=wireless%2Bkeyboard%2Band%2Bmouse&qid=1719355777&sprefix=wireless%2Bkeyboard%2Band%2Bmouse%2Caps%2C207&sr=8-3&th=1"> Link </a> |
| Basic connections components kit | Contains breadboards, resistors, LEDs, and jumper wires | $11.99 | <a href="https://www.amazon.com/Smraza-Breadboard-Resistors-Mega2560-Raspberry/dp/B01HRR7EBG/ref=sr_1_16?crid=27G99F3EADUCG&keywords=breadboard+1+pc&qid=1689894556&sprefix=breadboard+1+p%2Caps%2C185&sr=8-16"> Link </a> |


<!--
# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
-->

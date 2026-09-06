
**Interested in building your own?**
**Firmware, DIY kits, and fully assembled Internet Radio Units are available at:** [https://tmicromaker.com/](https://tmicromaker.com/)


This is a fully functional Internet Radio Based on ESP32-S3

![IMG_3577](https://github.com/user-attachments/assets/19e128bc-b9b6-4e2b-bd15-aea5ab638663)

![IMG_3576](https://github.com/user-attachments/assets/ca0a1ff1-3cd8-4685-a9a8-28e3d01f89e3)

<img width="4032" height="2268" alt="IMG_4994" src="https://github.com/user-attachments/assets/b02f5701-7adf-4c5c-8062-8f69f8b3f6c6" />


![IMG_4870](https://github.com/user-attachments/assets/27eed72e-b462-4414-9c2e-7d4f0acef384)

Internet Radio Based on ESP32-P4 with SPDIF out and WebUi Management Interface

![IMG_4602](https://github.com/user-attachments/assets/404d861e-c2d5-45e2-b299-c588e6edba75)

A repository where you can find documantation, various firmware version and enclosures 3D files, : 
https://tinyurl.com/4yduvmdj

<img width="228" height="228" alt="image" src="https://github.com/user-attachments/assets/e6c9b7a2-3e71-4442-8183-ced2320a94c2" />

For any quations Email me to: tmicromaker@gmail.com

Note: The Radio was designed to work only with ESP32S3 Lilygo t-displayS3 Touch or an ESP32-S3 and 170x320 touch screen that share the same caracteristics


You can watch the Radio various versions and evolution here:

**https://www.youtube.com/@tmicromaker**



**Installation:**

In your web prowser open:  https://micromkr.github.io/firmware/MicroMaker-Flasher.html

<img width="637" height="910" alt="image" src="https://github.com/user-attachments/assets/e07d45e6-6b3a-440c-8eab-9815db43fa2c" />


Connect your microcontroller to the USB port of your computer.

Choose the right firmware

Press connect choose the right port and flash.

After flashing is finished:

Press the RESET button on the ESP board (if it does not reboot automatically).

The new firmware will start running.

After ESP32 boot wait for few min until network scanning is completed.
Open the wifi in your phone and search for BT_Radio
Connect to your network
Wait for 5 minutes for the files system format to be completed
(You might need to turn off/on the radio) Look at the LCD for the IP address
connect to that IP address using your computer browser
Upload a single station or list of stations using the following format

Station Name 1,Station Address 1

Station Name 2,Station Address 2

Radio Space,http://123.456.789.0/stream

Radio Hits,http://stream.awesomehitsradio.com
.
Note: An I2S DAC is required for this project, Amplifier is optional.  Consult the I2S data sheet to learn how to activate the (L+R)/2 or stereo signal.  

Note: for some stations that don't play and their URL starts with https:// try to change it to http:// and check if it is working

Connection diagram using the Max98357a chip (if you use a header you don't need to connect wires as the pins are arranged correctly). 
I strongly recommend using the PCM5102a for better sound quality.      
 
Connect the I2S DAC to the following pins: 
BCLK to pin 12, 
LRC to pin 11, 
DOUT to pin 13,
VCC to 5V,
GND to GND

Following is the connection diagram:
![2000](https://github.com/Arielhh/ESP32-Radio-Internet/assets/4849568/eb7a9487-50be-4602-b988-5af08c9675d4)

Just solder it like that and connect it to the speaker (the pins are already aligned with the DAC pins):


![2001](https://github.com/Arielhh/ESP32-Radio-Internet/assets/4849568/cfae9a96-6d9e-48fd-bd41-e1cd02ca62a5)


![image](https://github.com/Arielhh/ESP32-Radio-Internet/assets/4849568/d405b0ce-b7a1-45ff-980c-08a1a25e7c60)
![image](https://github.com/Arielhh/ESP32-Radio-Internet/assets/4849568/d6fd0191-0bdb-4603-8089-db5a063e00e1)

Optional Pam8406 amplifier 2x6w amp+ pcm5102a Stereo DAC on one PCB which can be mounted directlly on top of the LILYGO T-Display Touch S3 (no wires soldering needed)
![pam](https://github.com/user-attachments/assets/7c26c655-e0bc-49e2-af36-5a40c3ad6195)



There is also a bluetooth streamer version (without a speaker):
![IMG_4067](https://github.com/user-attachments/assets/a20ece25-72aa-4b3f-93ca-11b82eedc690)

![IMG_E4071](https://github.com/user-attachments/assets/1cafccae-8f19-4aa5-95db-807c45a0d5f8)


<img width="1139" height="757" alt="BTModule1" src="https://github.com/user-attachments/assets/d68579f1-50c5-45b5-9e58-e8899d4142c4" />

You can watch the videos by clicking on the below videos:


[![▶ Watch the video](https://i9.ytimg.com/vi_webp/UsdidMPg164/mqdefault.webp?v=69a4ca24&sqp=CKCTk80G&rs=AOn4CLAiW8gmMZz_3K2KjQ3we_rY3myKoQ)](https://youtu.be/UsdidMPg164)


[![▶ Watch the video](https://i9.ytimg.com/vi_webp/jb2SspnF-nk/mqdefault.webp?v=69a4c9dd&sqp=CKSak80G&rs=AOn4CLA0-gdPMe77tKCUpStJ2oLFzjOb8A)](https://youtu.be/jb2SspnF-nk)



<img width="960" height="2079" alt="IMG_4120" src="https://github.com/user-attachments/assets/25ca0843-2f65-4cc2-a37c-2d5a26b93e64" />


<img width="960" height="2079" alt="IMG_4119" src="https://github.com/user-attachments/assets/05e602a6-6c70-4f35-9cd4-3f1f6bd80f06" />


<img width="960" height="2079" alt="IMG_4118" src="https://github.com/user-attachments/assets/533ca806-4d90-4311-9fdc-9479be0be163" />


<img width="960" height="2079" alt="IMG_4117" src="https://github.com/user-attachments/assets/ed21bb34-0ba5-46ee-ae3a-978e6f882bd2" />


<img width="960" height="2079" alt="IMG_4116" src="https://github.com/user-attachments/assets/d86291b0-c3cf-4f3c-a790-0854d6250496" />














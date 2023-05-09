# Comparing `tmp/image-to-arduino-1.0.4.1.tar.gz` & `tmp/image-to-arduino-1.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.4.1.tar", last modified: Sun May  7 13:20:10 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.4.2.tar", last modified: Tue May  9 16:03:21 2023, max compression
```

## Comparing `image-to-arduino-1.0.4.1.tar` & `image-to-arduino-1.0.4.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 13:20:10.751767 image-to-arduino-1.0.4.1/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.4.1/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 10:45:25.000000 image-to-arduino-1.0.4.1/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 13:20:10.751767 image-to-arduino-1.0.4.1/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.4.1/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 13:20:10.751767 image-to-arduino-1.0.4.1/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 13:20:10.000000 image-to-arduino-1.0.4.1/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      335 2023-05-07 13:20:10.000000 image-to-arduino-1.0.4.1/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 13:20:10.000000 image-to-arduino-1.0.4.1/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       61 2023-05-07 13:20:10.000000 image-to-arduino-1.0.4.1/image_to_arduino.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 13:20:10.000000 image-to-arduino-1.0.4.1/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 13:20:10.000000 image-to-arduino-1.0.4.1/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-04-22 13:23:37.000000 image-to-arduino-1.0.4.1/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 13:20:10.751767 image-to-arduino-1.0.4.1/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1156 2023-05-07 13:19:37.000000 image-to-arduino-1.0.4.1/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 13:20:10.751767 image-to-arduino-1.0.4.1/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 13:17:08.000000 image-to-arduino-1.0.4.1/src/__init__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     8369 2023-05-07 13:13:54.000000 image-to-arduino-1.0.4.1/src/imagetoarduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2324 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      374 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       66 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       15 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/top_level.txt
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/imagetoarduino/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/imagetoarduino/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       61 2023-05-09 15:55:50.000000 image-to-arduino-1.0.4.2/imagetoarduino/__main__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     8265 2023-05-09 15:59:47.000000 image-to-arduino-1.0.4.2/imagetoarduino/main.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1183 2023-05-09 16:02:25.000000 image-to-arduino-1.0.4.2/setup.py
```

### Comparing `image-to-arduino-1.0.4.1/LICENSE` & `image-to-arduino-1.0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.4.1/README.md` & `image-to-arduino-1.0.4.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,42 @@
 # Image Converter GUI APP for Arduino oled display ssd1306 128x64
 ## About Project
-Application has been created in order to easy convert image into your <strong>Arduino</strong> project with <strong>oled displays</strong>
+Application has been created in order to easy convert images into your <strong>Arduino</strong> project with <strong>oled displays</strong>
 ### How does it work:
 While you open .png and .jpg (others extensions in the future) image in app, the algorithm convert it to hexdeicmal array. Then it             returns full     code, ready to copy and put into the Arduino IDE. You can also preview how image will you like on your dislplay
 ## Demo
  <p align="center">
 <img src="https://user-images.githubusercontent.com/123249470/232137289-ff2707a7-a4bf-4e55-88a5-a469f54c3c3d.gif" width="350" height="560">
 </p>
 
-## How to install
-#### First of all download python and pip and check version
+## Getting Started
+### Prerequisites
+Download python, pip and check version
 ```
-pip3 --version 
-python --version
-```
-
-### Windows:
-Type into CMD:
-```
-pip3 install image-to-arduino
+$ pip3 --version 
+$ python --version
 ```
-```
-pip3 install tk
-```
-### Linux: 
+### Installation
+#### Windows/Linux/Mac OS:
 ```
 $ pip3 install image-to-arduino
+$ image-to-arduino
 ```
+### How to upgrade version
+#### Windows/Linux/Mac OS:
 ```
-$ sudo apt-get install python3-tk
-```
-### Mac OS:
-```
-~ % pip3 install image-to-arduino
-```
-```
-~ % pip3 install tk 
-```
-## How to run
-```
-$ pip3 show image-to-arduino
-```
-copy location path and add ```/src``` to the end
-```
-$ cd <copyied path/src>
-```
-### For example:
-```
-$ pip3 show image-to-arduino
-Location: /home/usr/Image_Converter_App
-$ cd /home/usr/Image_Converter_App/src
-```
-### Windows:
-#### Run the script:
-```
-python image_to_arduino.py
-```
-### Linux/Mac OS:
-#### Mark the file as an executable:
-```
-$ chmod +x image_to_arduino.py 
-```
-#### Run the script:
-```
-$ python3 image_to_arduino.py 
+$ pip3 install --upgrade image-to-arduino
 ```
 ## How to connect display to Arduino
 
 <p align="center">
       <img src="https://user-images.githubusercontent.com/123249470/233432819-97b593ab-d380-4945-85ab-543dbb49921b.png" width="620" height="480">
 </p>
 
-IMPORTANT: If you have Arduino board with inputs SCK and SDA, use them instead of A4 and A5 inputs
+<strong>IMPORTANT:</strong> If you have Arduino board with inputs SCK and SDA, use them instead of A4 and A5 inputs
 
 ## How to Contribute
 1. Fork the Project
 2. Clone repo with your GitHub username instead of ```YOUR-USERNAME```:<br>
 ```
 $ git clone https://github.com/YOUR-USERNAME/Image_Converter_App 
 ```
@@ -91,21 +52,21 @@
 * <del> upgrade graphics and style </del><br>
 * <del> add more functions </del><br>
 * add more than one display size<br>
 * make icon of the app<br>
 * <del> show preview of an image </del> <br>
 * make app as .exe <br>
 * <del> reverse color of image </del><br>
-* create function which generate full arduino code(not only arduino array) and connect it to switch button
+* <del> create function which generate full arduino code(not only arduino array) and connect it to switch button</del>
 ## What I have learned
 *	tkinter library skills 
 *	basics of UX and GUI
 *	image processing 
 ## Used libraries
 * tkinter 
 * customtkinter
 * openCV
 * numpy
 ## Version
-Version 1.0.3.1
+Version 1.0.3.2
 ## License 
 [MIT license](LICENSE)
```

### Comparing `image-to-arduino-1.0.4.1/setup.py` & `image-to-arduino-1.0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # Read the requirements.txt file and split into a list of lines
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 
 setup(
    name='image-to-arduino',
-   version='1.0.4.1',
+   version='1.0.4.2',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
-   packages=['src'],
-   package_data={'src': ['data/*.dat']},
+   packages=['imagetoarduino'],
+   package_data={'imagetoarduino': ['data/*.dat']},
    install_requires=REQUIREMENTS, 
     entry_points={
         'console_scripts': [
-            'image-to-arduino = src.imagetoarduino:main'
+            'image-to-arduino = imagetoarduino.__main__:main'
         ]
     },
 
 )
```

### Comparing `image-to-arduino-1.0.4.1/src/imagetoarduino.py` & `image-to-arduino-1.0.4.2/imagetoarduino/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 # To check extenxion
 import imghdr
 file_path = ''
 image_tk = ''
 left_switch_state = False
 right_switch_state = False
+
 def main():
 
     def open_file():
         global file_path
         file_path = filedialog.askopenfilename()
         if file_path:
             # If file name len is greater than 15: return ... + extension
@@ -81,31 +82,31 @@
 
                 if right_switch_state == False:
                     # Generate C++ array
                     cpp_array = 'const unsigned char PROGMEM ' + os.path.splitext(os.path.basename(file_path))[0] + ' [] = {\n' + cpp_array + '\n};' 
                 elif right_switch_state == True:
                     # Generate full code ready to use 
                     cpp_array = '''#include <Adafruit_SSD1306.h>
-    #include <Adafruit_GFX.h>
-    #define OLED_RESET 4
-    Adafruit_SSD1306 display(OLED_RESET);
-    const unsigned char PROGMEM ''' + os.path.splitext(os.path.basename(file_path))[0] + '''[] = {''' +  cpp_array + ''' };
-    void setup() 
-    {
-        display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
-        display.display();
-        delay(2000);
-        display.clearDisplay();}
-    void loop() 
-    {
-        display.drawBitmap(0, 0, ''' + os.path.splitext(os.path.basename(file_path))[0] + ''', 128, 64, 1); 
-        display.display();
-        delay(5000);
-        display.clearDisplay();
-        delay(5000);}'''        
+#include <Adafruit_GFX.h>
+#define OLED_RESET 4
+Adafruit_SSD1306 display(OLED_RESET);
+const unsigned char PROGMEM ''' + os.path.splitext(os.path.basename(file_path))[0] + '''[] = {\n''' +  cpp_array + ''' };
+void setup() 
+{
+    display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
+    display.display();
+    delay(2000);
+    display.clearDisplay();}
+void loop() 
+{
+    display.drawBitmap(0, 0, ''' + os.path.splitext(os.path.basename(file_path))[0] + ''', 128, 64, 1); 
+    display.display();
+    delay(5000);
+    display.clearDisplay();
+    delay(5000);}'''        
 
                 output_text.delete(1.0, tk.END)
                 output_text.insert(tk.END, cpp_array)
             
             # In case of error or invalid extension 
             except:
                 output_text.delete(1.0, tk.END)
@@ -190,10 +191,8 @@
     # "Clear all" button 
     clear_all_button = customtkinter.CTkButton(root, text="Clear All", command=clear_all)
     clear_all_button.grid(row=4, column=0, pady=5, padx=10, columnspan=1, sticky="nsew")  
 
     # Configure the window to not be resizable
     root.resizable(False, False)
 
-    root.mainloop()
-if __name__ == '__main__':
-    main()
+    root.mainloop()
```


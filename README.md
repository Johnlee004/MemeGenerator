# MemeGenerator

* [Purpose](#Purpose)
* [Objective](#Objective)
* [Possible Future Improvements](#Possible-Future-Improvements)
* [Imports](#Imports)
* [Features](#Features)
* [SetUps](#SetUps)
* [Credit](#Credit)

# Purpose
This program gets images links from a subchannel called r/Meme in a social media site called "reddit" then display them in the display page.

# Objective
This program was created to help myself better understand about API and the python library called "Requests", as well as a practical programming experience. This project also helped me understand about dynamic and static pagination and the solution to them.

# Possible Future Improvements
* Separate the UI code and the written code into two different py files
* Make the image display(pixel map) auto adjust size when the MainWindow changes its size
* Make a speed limit for requesting links so that requesting large amount of links is possible with longer time.

# Imports - all included in the venv folder
* random
* requests
* json
* urllib
* PyQt5
* time

# Features
![alt text](https://github.com/Johnlee004/images/blob/main/MemeGenerator-settingspage.PNG)
  ## Sort By:
  * has 4 elements in the dropbox: top, hot, new, and rising.

  ## Within:
  * has 4 elements in the dropbox: hour, week, year, and all.

  ## Repeat:
  * True: viewed image link won't be deleted(a chance to have the same image coming up again)
  * False: viewed image link will be deleted(no repetition)

  ## amount:
  * allows user to choose how many image link to request
  * removed due to spamming

  ## Generate:
  * load the image links to be viewed
  * 180 seconds cool download to avoid spamming

  ![alt text](https://github.com/Johnlee004/images/blob/main/MemeGenerator-display%20page.PNG)
  ## Download:
  * Download the displaying image as .png in the same directory.
  
  ## Next Image:
  * Randomly choose a image that was generated
    * if Repeat is false then the previous one will be delete(will never be viewed again).

# SetUps
* Download **.venv** folder and **MemeGenerator.py**.
* Start command prompt and activate the venv by executing the **activate.bat** file in **.venv\Scripts\activate.bat**
* Run the MemeGenerator within the venv.
* Set the setting to the preferred settings then click the **generate** button.
* Go to the display page by cicking the **display** button
* Click **Next Image** to start viewing them.

# Credit
The UI was created with PyQt5 designer and the UI code was converted from it. The UI file is in the repository.

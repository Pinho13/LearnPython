# Prerequisites

In this step, you will learn how to download and set up everything you need to get started with this guide. The instructions are written for Windows users, but if you are on a different operating system, the general ideas will still apply, even if the steps are slightly different.

## Python

Before anything else, you need Python installed. Python reads and understands your code and tells the computer what to do.

We will be using Python 3.12.0

### Setup:

* Go [here](https://www.python.org/downloads/release/python-3120/)
* Scroll to the bottom of the page
* Choose the correct version (from the table shown below)
![Versions](images/PythonVersions.png)
* Open the file downloaded and follow the instructions


## Code Editor

You also need a place to write your code. This can be almost anything (even your Notepad app) since, at its core, coding is simply writing text. However, there are tools designed to make coding easier and faster by helping you catch mistakes and write code more efficiently. These tools are called code editors.

The Code Editor I personally recommend is Visual Studio Code, a free and lightweight code editor developed by Microsoft.

<p align="center">
    <image src="images/VSCodeMeme.jpeg" width ="400px" />
</p>

### Setup:

* Download it [here](https://code.visualstudio.com/download)
* Open the file downloaded and follow the instructions
* Create a folder where you will store your python files (Scripts)
* Open Visual Studio Code
* Go to the top left where it says *File*
* Click it and click on *Open Folder*
* Select the folder created earlier
* In case this pops up, click there:
![I Trust](images/I_trust_myself_vscode.png)

### Adding the Python Extension

As you can see, there are a few icons on the left side of the screen. The first thing we want to click is the last icon, which is the Extensions icon.

VS Code allows us to install extensions. Extensions add extra features to the editor and can help us work more easily with specific programming languages.

Next, we want to install the Python extension. This extension adds helpful features such as code autocomplete while writing Python code, as well as other tools that make coding in Python easier.

![Python Extension](images/DownloadPythonExtension.png)

### Creating Our First Python File

Now that this is done, we can go and create our first python file. The first icon in the left opens up a tab that shows all of the current files in the folder open.

![Creating File](images/CreatingFile.png)

Since there are no files in the current folder, it is empty. To create a new file, click on the highlighted icon.

> Note: In the image, you may notice more icons on the left and different colors in VS Code. This is because I have additional extensions installed. If you’d like to customize your VS Code as well, feel free to look it up later.

After clicking the *New File* icon, name your file **test.py**. All python files should end with the **.py** extension.

Write this in the file (it will be explained later):

```py
print("Hello, world!")
```

Click on the run icon on the top right of the screen.

![Run Icon](images/RunIcon.png)

A notification will pop up asking you to choose the python interpreter. Choose the one available.

Once you see *Hello, world!* written in the bottom of the screen it means the setup is complete and you all the prerequisites necessary.

<p align="center">
    <image src="images/VSCodeNotTrustingMeMeme.png" width ="300px" />
</p>
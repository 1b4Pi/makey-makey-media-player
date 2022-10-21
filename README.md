# MakeyMakey Media Player Installation

A DGD-365 Application

## Step 1: Install Node.js

*As an asynchronous event-driven JavaScript runtime, Node.js is designed to build scalable network applications.*

Download the LTS version of [Node.js] (https://nodejs.org/)

## Step 2: Activate Yarn

*Yarn is a package manager for your code. It allows you to use and share code with other developers from around the world.*

### On Mac:

Open the /Applications/Utilities folder, then double-click Terminal.

### On PC:

1. Press the Start taskbar button.
2. Select All apps on the Start menu.
3. Scroll down the Start menu to the Windows Terminal app shown directly below.
4. Then click Windows Terminal there to open it. Alternatively, right-click it and select More > Run as administrator.

### Now that Terminal is open

Type the following in Terminal and press the Enter/Return key to activate Yarn:

```bash
corepack enable
```

## Step 3: Install Quasar

*Quasar is an MIT licensed open-source Vue.js based framework, which allows you as a web developer to quickly create responsive websites/apps in many flavors*

In your Terminal window, type the following command and press the Enter/Return key:

```bash
yarn global add @quasar/cli
```


## Step 4: Download and install the code for this app

On a Mac, you should have a folder called Sites inside your home directory, where the Desktop, Documents, and Downloads folders are located. If you don't have a folder called Sites here, make one.

Locate the **code** dropdown button at the top of this page and download the .zip file and move the uncompressed folder into your Sites directory.

Open a new terminal window and type the following command and press Enter/Return:

```bash
cd Sites/immersive-spaces
```

You are now inside the immersive-spaces folder. Run the following command to install the app:

```bash
yarn
```

### Step 5: Start the app in development mode (hot-code reloading, error reporting, etc.)

Make sure your Terminal window is inside the **immersive-spaces** folder (read step above)

```bash
quasar dev
```

# Remap your MakeyMakey

Follow this guide to remap your MakeyMakey inputs to use lowercase alphabet letters, starting with **a**. Your second input should be **b**. The third is **c**, and so on. You can take advantage of the back of the board to remap up to 18 inputs, which is the keyboard letter **r**.

# Customizing the MakeyMakey Media Player

Video files, and poster frames for each video file, are located in the **src/assets** folder.

This folder contains 18 videos with 18 poster frames. Each video & poster frame corresponds to a potential MakeyMakey input.

Update the media:
-Name your video and JPG files in the same manner as those in the src/assets/ folder and replace the old files with your new ones.

**Make sure to refresh your browser to see the changes!**

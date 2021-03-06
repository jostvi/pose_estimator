# pose_estimator
Pose estimation with AlwaysAI

## Setup
This app requires an alwaysAI account. Head to the [Sign up page](https://alwaysai.co/auth?register=true) if you don't have an account yet. Follow the instructions to install the alwaysAI tools on your development machine. There's also instructions on this wiki. 

Next, create an empty project to be used with this app. When you clone this repo, you can run aai app configure within the repo directory and your new project will appear in the list. Or you can choose to create a new project here. 

## Usage
Once the alwaysAI tools are installed on your development machine (or edge device if developing directly on it) you can run the following CLI commands:

#### Login to your AlwaysAI account through the CLI
```
aai user login
```

#### To set up the target device & install path
```
aai app configure
```

#### To install the app to your target
```
aai app install
```

BE AWARE! The "Install python dependencies"-part may take FOREVER, like 40+ mins.  

#### Create a .env file and add credentials according to .env_template

#### To start the app
```
aai app start
```

While running, you can access the video stream in a browser at localhost:5000 or through the IP-address of your device followed by the port number (:5000).

FUN FACT: You may need to restart the app sometimes if your'e not seeing any pose prints in the terminal. 

#### To close the app

The best way to stop the app right know is with Ctrl + C in the terminal. You can stop the streamer and the printer with the Stop-button in the browser app. But to stop the main thread, you'll need to use Ctrl + C. 

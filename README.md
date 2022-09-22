# dog-cat-classifier
# Image classification (dogs and cats)
This code represents the website, once the artificial intelligence model is created and trained with Python and Tensorflow, which is exported to "json" and "bin" files.
It can be used on the cell phone, just point the camera at the dog or cat you want to classify (it can be a computer image, a photo, or a real one), it does it all in the browser using Tensorflow.js.

## How to use it

### Download the repository
Download the repository wherever you like on your computer.

### Start a server in the folder
This project uses a Tensorflow.js model, which requires http/https access to load.
For that you can use any server, but here is a way to do it:
- Download Python to your computer
- Open a command line or terminal
- Navigate to the folder where you downloaded the repository
- Run the command `python -m http.server 8000`.
- Open a browser and go to http://localhost:8000

### Using it on a cell phone
If you want to open it on your cell phone, you can't just put in your computer's local IP and port, since HTTPS is required to use the camera. You can tunnel HTTPS by following these steps
- Download ngrok to your computer, and unzip it.
- Open a command line or terminal
- Navigate to the folder where you downloaded ngrok
- Run the command `ngrok http 8000`.
- It is important to have both active: the python server, and the ngrok tunnel.
- An HTTPS link will appear in the command line. You can log in there with your cell phone, no matter if you are not on the local network.
- The tunnel expires after 2 hours I think, in that case just restart ngrok.
- Open a browser on your cell phone and go to the HTTPS link indicated

### Usage
You can click on the "Change camera" button to use the front or back camera of your phone. Just point the camera at a dog or cat, and the prediction will appear below. It's not the future sorter either so if it doesn't sort perfect, oops.

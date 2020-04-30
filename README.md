# LiveStreamer
A simple client-server application to live stream the video captured via webcam/video file over the network.
We first establish a connection between the client and server and then start capturing the video frames using OpenCV module, serialize the image matrix using pickle and send the frame length and frame data to the server in respective order.
Server first receives the length of the frame data in a fixed length structs and then receives the complete frame.
It then coverts the received frame back to image mat and displays at the server side.

### Usage

Running the script without any arguments starts a server at localhost and default port.Run with a flag -c to run as a client. See other arguments in main func for other arg details.



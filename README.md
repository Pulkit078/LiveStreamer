# LiveStreamer
A simple client-server application to live stream the video captured via webcam/video file over the network.
We first establish a connection between the client and server and then start capturing the video frames using OpenCV module, serialize the image matrix and write the frame length and frame data to the stream in respective order.
Server first receives the length of the frame data in a fixed length structs and then receives the complete frame.
It then coverts the received frame back to image mat and displays at the server side.


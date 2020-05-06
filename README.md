# Udacity course Intel Edge AI for IoT Developers Nanodegree - Project 2 - Smart Qeueing

Write-up for this project is in the Choose the Right Hardware file.

## Stand-Out Suggestions
Once you're done with all of the required parts of your project, you can take it a step further and tinker with a few other hardware features! You can try out these standout suggestions. Note that these are all optional and are not required to pass the project.

There are some pointers given below. These will help you implement the stand out suggestions in your project

1. Multi-Device Plugin: Multi-Device plugin automatically assigns inference requests to available computational devices to execute the requests in parallel. You can use the multi-device plugin available as a part of the OpenVINO toolkit. When you submit your project, leave a brief note for your reviewer letting them know how you used the plugin.

The information or documentation on this can be found here
2. Heterogeneous Plugin: The heterogeneous plugin enables computing for inference on one network on several devices. You can use OpenVINO's Hetero plugin to use a fallback device like CPU when the main prediction device fails. When you submit your project, leave a brief note for your reviewer letting them know how you used the plugin.

More information regarding default or manual Fallback Policy can be found here


## Stand-out work
Overhead:

I found there was significant overhead with drawing the boxes and saving the video, for example on CPU for the Manufacturing project I saw:

FPS | Total Inference Time | Description
----|----------------------|-------------
 31 | 8.8 seconds          | normal inference and output
 60 | 4.6 seconds          | no drawing bboxes, no saving output video
212 | 1.3 seconds          | reading frames only




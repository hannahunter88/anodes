# Image Effect Scheduler Node Set for ComfyUI

ImageEffect nodes were created to provide complete control over visual effects by allowing users to specify individual values for each frame. For example it can be useful in creating visual effects that are synchronized with extracted music features.

ImageEffect nodes were also created to enable the creation of smoother, more consistent visual effects by automatically interpolating values between frames when users provide fewer specific values.

*Installation*

Clone this repo into custom_nodes folder.

*How to use these nodes?*

ImageEffect nodes should be applied after KSampler and VAE decode and before Preview Images and Video Combine nodes. 
It is also recommended to experiment with multiple ImageEffect nodes simultaneously, while keeping the original preview images and video for comparison.

Values in the list should be specified as floating-point numbers between 0 and 1. Use the multiplier parameter if you need higher values. For ImageEffectHue, the allowed range is -0.5 to 0.5, but these values are also rescaled to fit with the other ImageEffect Nodes, so you can still work with floating-point values between 0 and 1.


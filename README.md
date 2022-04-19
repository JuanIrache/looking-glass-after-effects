# looking-glass-after-effects

Create Looking Glass quilts from side tracking shots in Adobe After Effects. See [sample footage here](https://youtu.be/hQa8DnxfTOY).

## Prerequisites

- A [Looking Glass](https://lookingglassfactory.com/) holographic display
- Install [HoloPlay Service](https://lookingglassfactory.com/software#holoplay-service) to communicate with the device
- Install [HoloPlay Studio](https://lookingglassfactory.com/software) to load your work into the device
- Install [Adobe After Effects](https://www.adobe.com/products/aftereffects.html). Basic AE knowledge is required

## Instructions

Shoot video while constantly moving the camera along its transversal axis (i.e. left to right or right to left) in the most stable way possible: with a slider, drone, vehicle... Make sure the scene does not have many moving elements. The fewer the better. Then:

- Load your footage into the After Effects template
- Select a section of your footage that moves at a constant speed and drop it inside the **FOOTAGE** composition. If the resolution does not fill the entire comp, either rescale the footage or the composition. Either should work well as long as the result has a wider aspect ratio than the cells in the Quilt
- Open the **QUILT** composition, select the **SETTINGS** layer and go to the Effects Controls tab
- Set the right **Movement** direction of your shot
- Set the amount of **Depth**. This will require some trial and error. As a rule of thumb, the faster your movement the less depth you should apply. Depth actually means seconds between your first and last camera angles
- Set the **Focus** value. This determines the sharpest region of your shot. 0 will set the closest elements in focus and 100 will do so with the background. Find a moment where the most relevant element is on screen and adjust the slider until it is aligned vertically in all the cells. If you re-adjust the depth value, you will need to readjust focus as well. The higher the depth, the further the minimum focus point is, so if you cannot focus close enough, use a smaller depth. Potentially, you can set key frames and adjust the focus distance for different moments
- Adjust the work area of your composition to remove the last seconds of the footage, where cells start to disappear. The depth value will determine the number of seconds you need to trim
- Export your composition to one of the [compatible formats](https://docs.lookingglassfactory.com/keyconcepts/quilts#format)
- Plug your Looking Glass device and load your work with HoloPlay Studio

## Notes

- Orbiting shots may also work, but they can suffer from ["toe-in"](https://docs.lookingglassfactory.com/keyconcepts/camera#view-cone). When orbiting, high Focus values are probably better, in some cases even beyond 100, which you can set manually
- You can extend the duration of the FOOTAGE and QUILT compositions if necessary. Make sure to also extend the duration of hidden layers
- Currently this is designed to work witt the Looking Glass Portrait only
- Do not place layers above the **SETTINGS** one. That would break some important calculations
- You can use this to export still frames too, of course

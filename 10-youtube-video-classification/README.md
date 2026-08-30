## Project Summary

In this project, I built a **3D CNN model for video classification** using a subset of the UCF101 dataset. This was my first project working directly with video data, so the main goal was to understand the complete workflow, from processing video frames to training and evaluating a deep learning model.

The preprocessing pipeline included **frame sampling, resizing frames to 112×112 pixels, normalization, and changing the tensor format from `(Frames, Height, Width, Channels)` to `(Channels, Frames, Height, Width)`**, which is required by a 3D CNN. I used **32 frames per video** to provide the model with enough temporal information while keeping the training process reasonably efficient.

The dataset was divided into **training, validation, and test sets**. The model achieved around **100% training accuracy** and **92% validation accuracy**, but only **65.62% test accuracy**, indicating that the model has some difficulties generalizing to unseen videos.

The confusion matrix showed that **Punch** was classified particularly well, with 37 out of 39 videos correctly recognized. **CricketShot**, **PlayingCello**, and **ShavingBeard** also achieved relatively good results. The biggest challenge was **TennisSwing**, where only 9 out of 40 videos were classified correctly.

Overall, this project helped me understand the fundamentals of **video preprocessing, frame sampling, 3D CNN architecture, training and validation, and video classification evaluation**. Even though the model still has room for improvement, it demonstrates that a relatively simple 3D CNN can learn meaningful patterns from video data.
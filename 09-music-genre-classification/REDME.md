## Project Summary

In this project, I built a **CNN-based music genre classification model** using the **GTZAN music genre dataset**. This was my first project working directly with audio data, so the main goal was to understand how audio can be transformed into a format suitable for deep learning.

The audio files were loaded using **Librosa** and inspected by checking their sample rates and durations. The audio signals were then transformed into **Mel Spectrograms**, which represent the frequency content of the music over time while using a scale closer to human auditory perception. These spectrograms were normalized and prepared as input tensors for the CNN.

The dataset was split into **training, validation, and test sets**, and a PyTorch CNN was trained using **CrossEntropyLoss** and the **Adam optimizer**. Early stopping and saving the best model based on validation loss were also implemented to help prevent unnecessary training and overfitting.

The final model achieved approximately **57% test accuracy**. The confusion matrix showed that some genres, particularly **disco and rock**, were more difficult to distinguish, while **metal, pop, and country** were classified more successfully.

Although the dataset was relatively small and the CNN architecture was simple, the project demonstrates that a neural network can learn meaningful patterns from audio and classify music genres with reasonable accuracy. It also provided practical experience with an important audio-processing workflow: **raw audio → Mel Spectrogram → CNN → music genre prediction**.
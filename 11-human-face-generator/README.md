## Project Summary

In this project, I built a DCGAN capable of generating artificial human faces from random noise. The project allowed me to understand how GANs work by implementing both the Generator and Discriminator and training them in an adversarial process.

The Generator starts with a random latent vector and gradually transforms it into a 64×64 RGB image using transposed convolutional layers. The Discriminator takes both real images from the dataset and generated images and learns to distinguish between them. During training, the Generator learns from the feedback provided by the Discriminator and gradually improves the quality of the generated images.

After 50 epochs of training, the model was able to learn some basic characteristics of human faces, including oval face shapes, eyes, noses, hair, skin tones, and in some cases even basic facial expressions. However, many generated images were still distorted and unrealistic.

Although the final results were not as realistic as expected, this project was a valuable introduction to Generative Adversarial Networks. It helped me understand important concepts such as latent space, transposed convolutions, adversarial training, BCEWithLogitsLoss, gradient flow, and the use of `.detach()` when training the Discriminator.

Overall, the project demonstrated that even a relatively simple DCGAN can learn the general structure of human faces from a dataset, while also showing how challenging it is to achieve high-quality and realistic image generation.
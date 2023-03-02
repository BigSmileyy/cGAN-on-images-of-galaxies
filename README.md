# cGAN-on-images-of-galaxies
I use GAN to create galaxies that never existed. To do this, I will use the Galaxy10 dataset.
Galaxy10 - dataset containing 21785 69x69 px color images of galaxies divided into 10 classes.

<img width="815" alt="Снимок экрана 2023-03-02 в 14 52 40" src="https://user-images.githubusercontent.com/95381758/222421201-a6ac55ce-1c84-4e17-b175-28b8da48e622.png">

I want to generate each class individually.
In order to do this, you will need to use Conditional GAN (cGAN).

To make a cGAN out of a regular GAN, you need to somehow mix a class label into the latent vector. To do this, you need to convert the labels of the labels classes into a form that the neural network can work with (the conditional variable in the code) and mix them into inputs, forming conditional_inputs.

As a result, I received such images of galaxies for classes:

<img width="828" alt="Снимок экрана 2023-03-02 в 14 53 28" src="https://user-images.githubusercontent.com/95381758/222421369-481aa8cd-737c-486f-879d-bdeb5ebc8773.png">

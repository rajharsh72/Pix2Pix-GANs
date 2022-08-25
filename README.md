# What is Pix2Pix-GANs ?
    The Pix2Pix GAN is a general approach for image-to-image
    translation. It is based on the conditional generative adversarial network,
    where a target image is generated, conditional on a given input image. In
    this case, the Pix2Pix GAN changes the loss function so that the
    generated image is both plausible in the content of the target domain, and
    is a plausible translation of the input image. The Pix2Pix GAN was
    demonstrated on a wide variety of image generation tasks, including
    translating photographs from day to night and products sketches to
    photographs.

# Process/Methodology of my project:
    The Pix2Pix GAN architecture involves the careful
    specification of a generator model, discriminator model, and model
    optimization procedure. Both the generator and discriminator models use
    standard Convolution-Batch Normalization-ReLU blocks of layers as is
    common for deep convolutional neural networks.

# The generator :
    is trained via adversarial loss, which encourages the
    generator to generate plausible images in the target domain. The
    generator is also updated via L1 loss measured between the generated
    image and the expected output image. This additional loss encourages the
    generator model to create plausible translations of the source image.
    We will be using the so-called “maps” dataset. This is a dataset
    comprised of satellite images of New York and their corresponding
    Google maps pages. The image translation problem involves converting
    satellite photos to Google maps format, or the reverse, Google maps
    images to Satellite photos.

# The discriminator :
    is a deep convolutional neural network that performs
    image classification. Specifically, conditional-image classification. It
    Department of Information Technology
    takes both the source image (e.g. satellite photo) and the target image
    (e.g. Google maps image) as input and predicts the likelihood of whether
    target image is real or a fake translation of the source image.
    
    

# Output Images:
![image](https://user-images.githubusercontent.com/75540307/186744644-bd7127a3-31bb-4017-ae22-896a7504edfb.png)

![image](https://user-images.githubusercontent.com/75540307/186744774-a8033e34-acf0-40a2-a979-f8e2ed1bed2f.png)



# GenAI-A4

## Theory Questions

- Q1: Explain the minimax loss function in GANs and how it ensures competitive training
between the generator and discriminator.

The minimax loss function are the centerpiece for how GANs successfully train. GANs have two separate parts, the generator and the discriminator. The generator will generate data that tries to fool the discriminator, essentially minimizing its success rate. The discriminator attempts to distinguish between real and fake data trying to maximize its success rate.


- Q2: What is mode collapse, Why can mode collapse occur during GAN training? and
how can it be mitigated?

Mode collapse occurs the generator only produces a limited variety of examples instead of a diverse set of realistic data. The generator finds it easier to trick the discriminator by generating the same samples that has already worked. Mode collapse can be mitigated by using a Wasserstein GAN, or techniques such as batch normalization and minibatch discrimination.


- Q3: Explain the role of the discriminator in adversarial training?

The discriminator attempts to distinguish between real and generated data. After receiving both real samples and generated samples, the discriminator attempts to minimize its classification error.


- Q4: How do metrics like IS and FID evaluate GAN performance?

IS evaluates the diversity and confidence of classification, but not necessarily realism. FID evaluates the realism of the images, but not the diversity. Both metrics use a pre-trained model to do this evaluation.
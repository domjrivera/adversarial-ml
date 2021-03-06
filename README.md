# Adversarial Machine Learning


## RATIONALE

Image classification (using Keras and TensorFlow) can be attacked using
different sorts of techniques, from 1-pixel injections to random noise added to
the source image.

Social networks, message boards, other websites will collect one's avatar
image, and some websites are already collecting these images to cross-reference
those and profile users using their avatar images.

One idea I am exploring is about providing a way for developers to temper with
image uploads, so they could protect their users' images a little bit better.
Original images could live at the service provider's end, but anything they
would expose publicly would be a "protected" (attacked) image.

Here's a list of adversarial attack and techniques preventing Machine Learning
tools from recognizing patterns they should recognize, making lives of image
harvesters a little harder than before.


## PAPERS


### Adversarial Patch (Tom B. Brown, Dandelion Mané, Aurko Roy, Martín Abadi, Justin Gilmer) – (2017/12/27)

[Link](http://arxiv.org/pdf/1712.09665)
<blockquote>
We present a method to create universal, robust, targeted adversarial image
patches in the real world. The patches are universal because they can be used
to attack any scene, robust because they work under a wide variety of
transformations, and targeted because they can cause a classifier to output any
target class. These adversarial patches can be printed, added to any scene,
photographed, and presented to image classifiers; even when the patches are
small, they cause the classifiers to ignore the other items in the scene and
report a chosen target class.
</blockquote>

### Practical Black-Box Attacks against Machine Learning (Nicolas Papernot, Patrick McDaniel, Ian Goodfellow, Somesh Jha, Z. Berkay Celik, Ananthram Swami) – (2016/02/08)

[Link](http://arxiv.org/pdf/1602.02697)
<blockquote>
Machine learning (ML) models, e.g., deep neural networks (DNNs), are
vulnerable to adversarial examples: malicious inputs modified to yield
erroneous model outputs, while appearing unmodified to human observers.
Potential attacks include having malicious content like malware identified as
legitimate or controlling vehicle behavior. Yet, all existing adversarial
example attacks require knowledge of either the model internals or its training
data. We introduce the first practical demonstration of an attacker controlling
a remotely hosted DNN with no such knowledge. Indeed, the only capability of
our black-box adversary is to observe labels given by the DNN to chosen inputs.
Our attack strategy consists in training a local model to substitute for the
target DNN, using inputs synthetically generated by an adversary and labeled by
the target DNN. We use the local substitute to craft adversarial examples, and
find that they are misclassified by the targeted DNN. To perform a real-world
and properly-blinded evaluation, we attack a DNN hosted by MetaMind, an online
deep learning API. We find that their DNN misclassifies 84.24% of the
adversarial examples crafted with our substitute. We demonstrate the general
applicability of our strategy to many ML techniques by conducting the same
attack against models hosted by Amazon and Google, using logistic regression
substitutes. They yield adversarial examples misclassified by Amazon and Google
at rates of 96.19% and 88.94%. We also find that this black-box attack strategy
is capable of evading defense strategies previously found to make adversarial
example crafting harder.
</blockquote>

### Explaining and Harnessing Adversarial Examples (Ian J. Goodfellow, Jonathon Shlens, Christian Szegedy) – (2014/12/20)

[Link](http://arxiv.org/pdf/1412.6572)
<blockquote>
Several machine learning models, including neural networks, consistently
misclassify adversarial examples---inputs formed by applying small but
intentionally worst-case perturbations to examples from the dataset, such that
the perturbed input results in the model outputting an incorrect answer with
high confidence. Early attempts at explaining this phenomenon focused on
nonlinearity and overfitting. We argue instead that the primary cause of neural
networks' vulnerability to adversarial perturbation is their linear nature.
This explanation is supported by new quantitative results while giving the
first explanation of the most intriguing fact about them: their generalization
across architectures and training sets. Moreover, this view yields a simple and
fast method of generating adversarial examples. Using this approach to provide
examples for adversarial training, we reduce the test set error of a maxout
network on the MNIST dataset.
</blockquote>

### Adversarial examples in the physical world (Alexey Kurakin, Ian Goodfellow, Samy Bengio) – (2016/07/08)

[Link](http://arxiv.org/pdf/1607.02533)
<blockquote>
Most existing machine learning classifiers are highly vulnerable to
adversarial examples. An adversarial example is a sample of input data which
has been modified very slightly in a way that is intended to cause a machine
learning classifier to misclassify it. In many cases, these modifications can
be so subtle that a human observer does not even notice the modification at
all, yet the classifier still makes a mistake. Adversarial examples pose
security concerns because they could be used to perform an attack on machine
learning systems, even if the adversary has no access to the underlying model.
Up to now, all previous work have assumed a threat model in which the adversary
can feed data directly into the machine learning classifier. This is not always
the case for systems operating in the physical world, for example those which
are using signals from cameras and other sensors as an input. This paper shows
that even in such physical world scenarios, machine learning systems are
vulnerable to adversarial examples. We demonstrate this by feeding adversarial
images obtained from cell-phone camera to an ImageNet Inception classifier and
measuring the classification accuracy of the system. We find that a large
fraction of adversarial examples are classified incorrectly even when perceived
through the camera.
</blockquote>

### Practical Black-Box Attacks against Machine Learning (Nicolas Papernot, Patrick McDaniel, Ian Goodfellow, Somesh Jha, Z. Berkay Celik, Ananthram Swami) – (2016/02/08)

[Link](http://arxiv.org/pdf/1602.02697)
<blockquote>
Machine learning (ML) models, e.g., deep neural networks (DNNs), are
vulnerable to adversarial examples: malicious inputs modified to yield
erroneous model outputs, while appearing unmodified to human observers.
Potential attacks include having malicious content like malware identified as
legitimate or controlling vehicle behavior. Yet, all existing adversarial
example attacks require knowledge of either the model internals or its training
data. We introduce the first practical demonstration of an attacker controlling
a remotely hosted DNN with no such knowledge. Indeed, the only capability of
our black-box adversary is to observe labels given by the DNN to chosen inputs.
Our attack strategy consists in training a local model to substitute for the
target DNN, using inputs synthetically generated by an adversary and labeled by
the target DNN. We use the local substitute to craft adversarial examples, and
find that they are misclassified by the targeted DNN. To perform a real-world
and properly-blinded evaluation, we attack a DNN hosted by MetaMind, an online
deep learning API. We find that their DNN misclassifies 84.24% of the
adversarial examples crafted with our substitute. We demonstrate the general
applicability of our strategy to many ML techniques by conducting the same
attack against models hosted by Amazon and Google, using logistic regression
substitutes. They yield adversarial examples misclassified by Amazon and Google
at rates of 96.19% and 88.94%. We also find that this black-box attack strategy
is capable of evading defense strategies previously found to make adversarial
example crafting harder.
</blockquote>

### Adversarial Attacks on Neural Network Policies (Sandy Huang, Nicolas Papernot, Ian Goodfellow, Yan Duan, Pieter Abbeel) – (2017/02/08)

[Link](http://arxiv.org/pdf/1702.02284)
<blockquote>

</blockquote>

### Vulnerability of Deep Reinforcement Learning to Policy Induction Attacks (Vahid Behzadan, Arslan Munir) – (2017/01/16)

[Link](http://arxiv.org/pdf/1701.04143)
<blockquote>
Deep learning classifiers are known to be inherently vulnerable to
manipulation by intentionally perturbed inputs, named adversarial examples. In
this work, we establish that reinforcement learning techniques based on Deep
Q-Networks (DQNs) are also vulnerable to adversarial input perturbations, and
verify the transferability of adversarial examples across different DQN models.
Furthermore, we present a novel class of attacks based on this vulnerability
that enable policy manipulation and induction in the learning process of DQNs.
We propose an attack mechanism that exploits the transferability of adversarial
examples to implement policy induction attacks on DQNs, and demonstrate its
efficacy and impact through experimental study of a game-learning scenario.
</blockquote>

### Adversarial Attacks Against Medical Deep Learning Systems (Samuel G. Finlayson, Isaac S. Kohane, Andrew L. Beam) – (2018/04/15)

[Link](https://arxiv.org/abs/1804.05296)
<blockquote>
The discovery of adversarial examples has raised concerns about the practical deployment of deep learning systems. In this paper, we argue that the field of medicine may be uniquely susceptible to adversarial attacks, both in terms of monetary incentives and technical vulnerability. To this end, we outline the healthcare economy and the incentives it creates for fraud, we extend adversarial attacks to three popular medical imaging tasks, and we provide concrete examples of how and why such attacks could be realistically carried out. For each of our representative medical deep learning classifiers, both white and black box attacks were both effective and human-imperceptible. We urge caution in employing deep learning systems in clinical settings, and encourage research into domain-specific defense strategies.
</blockquote>

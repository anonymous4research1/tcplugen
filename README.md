# Adding temporal musical controls on top of pretrained generative models

This repository is linked to our paper submission to the [ISMIR 25](https://ismir2025.ismir.net/) Conference. 

*this website is still under construction*


Recent advances in deep generative modeling have enabled high-quality models for musical audio synthesis. 
However, these approaches remain difficult to control, confined to simple, static attributes and, most 
importantly, entail retraining a different computationally-heavy architecture for each new control. 
This is inefficient and impractical as it requires substantial computational resources.

In this paper, we propose a novel approach allowing to add time-varying musical controls on top of any 
pretrained generative models with an exposed latent space (e.g. neural audio codecs), without retraining or 
finetuning. Our method supports both discrete and continuous attributes by adapting a rectified flow approach 
with a latent diffusion transformer. We learn an invertible mapping between pretrained latent variables and 
a new space disentangling explicit control attributes and *style* variables that capture the remaining 
factors of variation.
This enables both feature extraction from an input, but also editing those features to generate transformed audio samples. 
Finally, this also introduces the ability to perform synthesis directly from the audio descriptors. 
We validate our method with 4 datasets going from different musical instruments up to full music recordings, 
on which we outperform state-of-the-art task-specific baselines in terms of both generation quality and accuracy 
of the control by inferring transferred attributes.

# Speckle correlation using Deep Learning on Newtonian fluids

Newtonian fluids such as water with predictable viscosity can be used to perform Dynamic Light Scattering. DLS is used to determine particle size and profiling of polymers in suspension that follow Brownian motion. This relation between the speed of the particles and size is related by the Stokes-Einstein equation.

$$D = \dfrac{k_BT}{6πηRH}$$

T = translational diffusion coefficient, T = temperature, η = viscosity, RH = hydrodynamic radius

In DLS, a source of monochromatic light, usually a Laser beam, is projected onto a fluid sample at a fixed distance. The laser beam striking the fluid produces a speckle pattern on fast photon counter at the far end. Time-dependent fluctuations in the scattered light measurement allows us to classify the profile of the impurity within the sample. Since the fluctuations are directly related to the diffusion rate of the particles in the sample, we charted a catalogue of impurities including not limited to the Lake Michigan water, sulphate-rich water, pure water and so on.

Previous experiments sought traditional data analysis approach where individual speckle patterns were evaluated per size distribution. Such methods of one-to-one mapping are computationally intensive and not generalised to seek larger relationships amongst different speckle patterns. In addition, sample pertur- bations could produce significantly different results. Other groups have, in fact, used Deep Learning aimed and achieved similar results as what we are investigating. The key difference is in the experiment, we used numerous Newtonian fluid samples from different sizes, qualities with pure water as a control. A Boston group tested on diffusers with homologous profiles, ours is heterogeneous in distribution.

A Convolutional Neural Network is a Deep Learning neural network designed for processing structured data arrays such as image. The usage of convolutional layers in a CNN mirrors the structure of the human visual cortex, where a series of layers process an incoming image and identify progressively more complex features. An image is a 2-dimensional array of pixels that can be classified based on its features. Our speckle data is an image data, each row is time-stamped and individual columns a different sample type. The data is randomly split into 70% training and 30% testing sets and later on cross-validated. We apply a CNN model because they very exceptional at picking up on patterns in the input image, such as lines, edges, and gradients. The gradient is the key one as speckles are low resolution images evolving over time. Each particle has its characteristic speckle profile that our deep learning model is able to pick up and quicker and at a higher rate of accuracy.

Using CNN, we can classify more types of impurities than traditional classification and labelling of the im- purities within fluids. This method is scalable and impactful in impurity testing as well as in characterising proteins, polymers, parasitic presence, etc. Drug industry and marine habitat could use such algorithms for enhancing quality control. My thesis is projected to use at least ten samples of fluids with different particles in suspension going. To best of our knowledge, our testing is of higher quality than other studies given our data incorporates diversity of samples, sensitivity tests and accuracy measurements.

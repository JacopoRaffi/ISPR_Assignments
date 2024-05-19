# ISPR_Assignments
Midterm assignments given during the Intelligent System for Pattern Recognition(ISPR) course.

## Assignment 1:
The musical pitch of a note is determined by its fundamental frequency. The pitch played by different instruments sounds different due to harmonics, i.e. other frequencies that are superimposed and determine the timbre of the instrument. [This dataset](https://philharmonia.co.uk/resources/sound-samples/) contains samples from several instruments playing different notes. Plot the spectrogram for some of them (4 instruments are sufficient) and check if it is possible to recognize the different instruments by only looking at the spectrogram. In your presentation, discuss which samples you chose to compare, how you computed the spectrogram and whether the resulting features are sufficient to recognize the instrument.

## Assignment 2:
Fit an Hidden Markov Model to the data in [DSET1](https://archive.ics.uci.edu/dataset/360/air+quality): it is sufficient to focus on a single column of the dataset of your choice (i.e. choose one of the sensors available and focus on analysis that single sensor). Experiment with training  HMMs with two different choices of the emission distribution and confront the results. Experiment also with HMMs with a varying number of hidden states (e.g. at least 2, 3 and 4) and identify what is the best choice according to your own reasoning. 

Once you have identified the best HMM configuration (emissions and number of states), choose a reasonably sized subsequence (e.g. last 25% of the timeseries) and compute the optimal assignement using two methods: 

1. Viterbi (true optimal); 
2. Best state according to the hidden state posterior (very local decision). 

Then plot the timeseries data highlighting (e.g. with different colours) the hidden state assigned to each timepoint by the Viterbi algorithm and the posterior method. Discuss the results.

## Assignment 3:
Train 1 denoising and 1 contractive autoencoder on the MNIST dataset. It is up to you to decide how many layers and neurons in each layer you want in the deep autoencoder. Show an accuracy comparison between the different autoencoders.

Then, experiment with what happens if you feed the autoencoders with a random noise image and then you apply the iterative gradient ascent process described in the lecture to see if the reconstruction converges to the data manifold. Confront the reconstructions created by the 2 different models and comment on the results.

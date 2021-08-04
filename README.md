# Overview
To predict the next frame based on the visual features from previous frames of a video using
Convolutional Long Short Term Memory (ConvLSTM).

# Architecture

The first module is video segmentation which converts the input video into video frames.
The segmented frames are stored in an 2D array. LSTM networks are a special kind of RNN,
capable of learning long-term dependencies. The video frames are sent one frame at a time to
the second module i.e. ConvLSTM model and it extracts the features of first frame, stores it
School of Computer Science & Engineering, KLE Technological University, Hubballi - 31. 9
Next Frame Prediction
and takes the next input frame. It predicts the next frame using the features in LSTM memory
cells. In third module, to analyze the frame predicted, we compare it with the Ground Truth
data.


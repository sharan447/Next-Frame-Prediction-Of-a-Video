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


![](Next%20Frame%20Prediction/Images/1.JPG)

The ConvLSTM model is split into two sections: one for reading the input sequence and
encoding it into a fixed-length vector, and the other for decoding the fixed-length vector and
predicting the sequence. The encoder generates a two-dimensional matrix of outputs, the
length of which is determined by the number of memory cells in the layer. The decoder is an
LSTM layer that expects a 3D input of [samples, time steps, features] and produces a decoded
sequence of a length determined by the task.


# Results

This consists of the samples taken from the dataset’s each category and shows the result
attained. The first five frames are the input frames taken from the videos segmented from the
dataset and the sixth frame is the predicted next frame i.e. the output generated from our
ConvLSTM model.


![](Next%20Frame%20Prediction/Images/2.JPG)


![](Next%20Frame%20Prediction/Images/3.JPG)


--About_deeplearning--

# What is Deep learning ? 
# Why we use deep learning ? 
# What is the main fundamental inside in deep learning ?
# Why deep learning learning so hard ? 
#


"Hello friends, my name is shyamal kar. in this  repository i gonna cover all deep learning topics , which are most important in deep learning. "

"Major architecture / model family"


1. ANN
    │
    ├── Neuron / Perceptron
    ├── Input / Hidden / Output Layers
    ├── Weights & Bias
    ├── Forward Propagation
    ├── Activation Functions
    │   ├── Sigmoid
    │   ├── Tanh
    │   ├── ReLU
    │   ├── Leaky ReLU
    │   ├── GELU
    │   └── Softmax
    ├── Loss Functions
    │   ├── MSE
    │   ├── MAE
    │   ├── Binary Cross Entropy
    │   └── Categorical Cross Entropy
    ├── Backpropagation
    ├── Gradient Descent
    ├── Optimizers
    │   ├── SGD
    │   ├── Momentum
    │   ├── RMSprop
    │   ├── Adam
    │   └── AdamW
    ├── Weight Initialization 
    │   ├── Xavier/Glorot
    │   └── He
    ├── Regularization
    │   ├── L1
    │   ├── L2
    │   ├── Dropout
    │   └── Early Stopping
    └── Batch Normalization

2. CNN (Convolutional neural network)
    │
    ├── Image Representation
    ├── Convolution
    │   ├── Kernel / Filter
    │   ├── Stride
    │   └── Padding
    ├── Feature Map
    ├── Activation
    ├── Pooling
    │   ├── Max Pooling
    │   └── Average Pooling
    ├── Flattening
    ├── Fully Connected Layer
    │
    ├── CNN Architectures
    │   ├── LeNet
    │   ├── AlexNet
    │   ├── VGG
    │   ├── Inception / GoogLeNet
    │   ├── ResNet
    │   ├── DenseNet
    │   ├── MobileNet
    │   └── EfficientNet
    │
    ├── Transfer Learning
    └── Computer Vision
        ├── Classification
        ├── Object Detection
        └── Segmentation

3. RNN

    │
    ├── Sequential Data
    ├── Hidden State
    ├── Recurrent Connection
    ├── Vanilla RNN
    │
    ├── Problems
    │   ├── Vanishing Gradient
    │   └── Exploding Gradient
    │
    ├── LSTM
    │   ├── Forget Gate
    │   ├── Input Gate
    │   ├── Output Gate
    │   └── Cell State
    │
    ├── GRU
    │   ├── Update Gate
    │   └── Reset Gate
    │
    ├── Bidirectional RNN
    ├── Bidirectional LSTM
    ├── Seq2Seq
    └── Encoder-Decoder

4. transformer

    │
    ├── Attention
    │   ├── Query
    │   ├── Key
    │   └── Value
    │
    ├── Self-Attention
    ├── Cross-Attention
    ├── Multi-Head Attention
    ├── Positional Encoding
    │
    ├── Feed Forward Network
    ├── Residual Connection
    ├── Layer Normalization
    │
    ├── Encoder
    ├── Decoder
    └── Transformer Architecture
        │
        ├── Encoder-only
        │   └── BERT
        │
        ├── Decoder-only
        │   └── GPT
        │
        └── Encoder-Decoder
            └── T5


5. GAN

    │
    ├── Generator
    ├── Discriminator
    ├── Adversarial Training
    ├── GAN Loss
    │
    ├── Training Process
    │
    ├── Problems
    │   ├── Mode Collapse
    │   └── Training Instability
    │
    ├── DCGAN
    ├── Conditional GAN
    └── StyleGAN

6. diffusion

    │
    ├── Forward Diffusion
    │   └── Add Noise
    │
    ├── Reverse Diffusion
    │   └── Remove Noise
    │
    ├── Noise Schedule
    ├── Noise Prediction
    ├── Denoising
    ├── DDPM
    ├── Conditioning
    ├── Text-to-Image
    └── Latent Diffusion
        └── Stable Diffusion-type systems

# Don't be afraid, we are clearing all these topics because later, as soon as there is a shift in the domain, we will study which ones we need to study more. We will study them again at the time of fear.


# But the question remain :-
# What is our study rule would be and what is the most priority topics we revise again ? 


# Our study rule would be :- 

1. pick a one topic,
2. what is this ?
3. why create this ? like = Using ANN it's very hard to handle spatial structure efficiently so we use CNN

4. How work inside ? here we go depth as copare to ML = 
Image
↓
Kernel
↓
Convolution
↓
Feature Map
↓
Activation
↓
Pooling
↓
Next Layer

5. Transformer
Input
↓
Q/K/V
↓
Attention
↓
Multi-Head Attention
↓
FFN
↓
Residual + LayerNorm
↓
Output

6. Math 
# try to understand how formula to computation understand this.

e.g.,  z = Wx + b

then :- 

a = f(z)

then loss :- L(y,^y )

then gradient :- 
∂W
∂L
# then weight update

	​W = W − η ∂W/∂L​

7. When to use ?

CNN -> sequential / spatial data
RNN -> sequential data
Transformer → language/sequence/attention-based problems
GAN → generative modeling
Diffusion → generative modeling

8. when not to use ?
for little tabular dataset CNN is generally not a logical first choice.

9. components 

CNN :- 

Kernel
Stride
Padding
Pooling
Channels
Feature Maps

Transformer :- 
Q
K
V
Attention Heads
Embedding
Positional Encoding
FFN
LayerNorm
Residual

10. architecture diagram 

# each architechture draw by my hand in khata. 

ANN :- 

Input
 ↓
Hidden Layer
 ↓
Output

CNN:-
Image
 ↓
Conv
 ↓
Pooling
 ↓
Conv
 ↓
Flatten
 ↓
Dense

transformer :- 

Embedding
 ↓
Attention
 ↓
FFN
 ↓
Output

11. Code 

From scratch/basic implementation → TensorFlow/Keras/PyTorch

ANN → scratching is very useful
Backpropagation → scratching is useful
CNN convolution → basic implementation useful
Attention → numerical/basic implementation is very useful
Transformer block → basic implementation is very useful
GAN → basic implementation
Diffusion → simplified implementation

12. Dataset / Practical 

# Do pratical same as ML 
# but depend on data architecture

ANN → Tabular dataset
CNN → Image dataset
RNN/LSTM → Sequence/Text/Time-series
Transformer → Text/Sequence
GAN → Image generation
Diffusion → Image generation

# Real world use case :- Where use in reality 

CNN → medical image classification
LSTM → time-series forecasting
Transformer → LLM
GAN → synthetic image generation
Diffusion → text-to-image


Conclusion :- 

In machine learning we often ask what do this algorithm but here i write why algorithm made for this ? 

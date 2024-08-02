# Computer Vision

Computer vision is one of the core areas of artificial intelligence (AI), and focuses on creating solutions that enable AI applications to "see" the world and make sense of it.

The ability to use filters to apply effects to images is useful in image processing tasks, such as you might perform with image editing software. However, the goal of computer vision is often to extract meaning, or at least actionable insights, from images; which requires the creation of machine learning models that are trained to recognize features based on large volumes of existing images.

Convolutional neural networks (CNNs)
One of the most common machine learning model architectures for computer vision is a convolutional neural network (CNN), a type of deep learning architecture. CNNs use filters to extract numeric feature maps from images, and then feed the feature values into a deep learning model to generate a label prediction. For example, in an image classification scenario, the label represents the main subject of the image (in other words, what is this an image of?). You might train a CNN model with images of different kinds of fruit (such as apple, banana, and orange) so that the label that is predicted is the type of fruit in a given image.

During the training process for a CNN, filter kernels are initially defined using randomly generated weight values. Then, as the training process progresses, the models predictions are evaluated against known label values, and the filter weights are adjusted to improve accuracy. Eventually, the trained fruit image classification model uses the filter weights that best extract features that help identify different kinds of fruit.

Transformers
Most advances in computer vision over the decades have been driven by improvements in CNN-based models. However, in another AI discipline - natural language processing (NLP), another type of neural network architecture, called a transformer has enabled the development of sophisticated models for language. Transformers work by processing huge volumes of data, and encoding language tokens (representing individual words or phrases) as vector-based embeddings (arrays of numeric values). You can think of an embedding as representing a set of dimensions that each represent some semantic attribute of the token. The embeddings are created such that tokens that are commonly used in the same context are closer together dimensionally than unrelated words.

Multi-modal models
The success of transformers as a way to build language models has led AI researchers to consider whether the same approach would be effective for image data. The result is the development of multi-modal models, in which the model is trained using a large volume of captioned images, with no fixed labels. An image encoder extracts features from images based on pixel values and combines them with text embeddings created by a language encoder. The overall model encapsulates relationships between natural language token embeddings and image features

Image classification: Identifying to which category an image belongs.
Object detection: Locating individual objects within an image.
Captioning: Generating appropriate descriptions of images.
Tagging: Compiling a list of relevant text tags for an image.

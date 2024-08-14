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

## Azure AI Vision

Microsoft's Azure AI Vision service provides prebuilt and customizable computer vision models that are based on the Florence foundation model and provide various powerful capabilities. With Azure AI Vision, you can create sophisticated computer vision solutions quickly and easily; taking advantage of "off-the-shelf" functionality for many common computer vision scenarios, while retaining the ability to create custom models using your own images.

### Azure resources for Azure AI Vision service

To use Azure AI Vision, you need to create a resource for it in your Azure subscription. You can use either of the following resource types:

Azure AI Vision: A specific resource for the Azure AI Vision service. Use this resource type if you don't intend to use any other Azure AI services, or if you want to track utilization and costs for your Azure AI Vision resource separately.

Azure AI services: A general resource that includes Azure AI Vision along with many other Azure AI services; such as Azure AI Language, Azure AI Custom Vision, Azure AI Translator, and others. Use this resource type if you plan to use multiple AI services and want to simplify administration and development.

#### Analyzing images with the Azure AI Vision service

After you've created a suitable resource in your subscription, you can submit images to the Azure AI Vision service to perform a wide range of analytical tasks.

Azure AI Vision supports multiple image analysis capabilities, including:

Optical character recognition (OCR) - extracting text from images.
Generating captions and descriptions of images.
Detection of thousands of common objects in images.
Tagging visual features in images

https://portal.vision.cognitive.azure.com/gallery/featured

Optical character recognition
Azure AI Vision service can use optical character recognition (OCR) capabilities to detect text in images.

Describing an image with captions
Azure AI Vision has the ability to analyze an image, evaluate the objects that are detected, and generate a human-readable phrase or sentence that can describe what was detected in the image.

Detecting common objects in an image
Azure AI Vision can identify thousands of common objects in images.

Tagging visual features
Azure AI Vision can suggest tags for an image based on its contents. These tags can be associated with the image as metadata that summarizes attributes of the image and can be useful if you want to index an image along with a set of key terms that might be used to search for images with specific attributes or contents.

Training custom models
If the built-in models provided by Azure AI Vision don't meet your needs, you can use the service to train a custom model for image classification or object detection.

Image classification
An image classification model is used to predict the category, or class of an image.

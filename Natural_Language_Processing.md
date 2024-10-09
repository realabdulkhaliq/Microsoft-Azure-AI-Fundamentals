# Natural Language Processing

Natural language processing supports applications that can see, hear, speak with, and understand users. Using text analytics, translation, and language understanding services, Microsoft Azure makes it easy to build applications that support natural language.

## Fundamentals of Text Analysis with the Language Service

Tokenization
The first step in analyzing a corpus is to break it down into tokens. For the sake of simplicity, you can think of each distinct word in the training text as a token, though in reality, tokens can be generated for partial words, or combinations of words and punctuation.

Frequency analysis
After tokenizing the words, you can perform some analysis to count the number of occurrences of each token. The most commonly used words (other than stop words such as "a", "the", and so on) can often provide a clue as to the main subject of a text corpus. For example, the most common words in the entire text of the "go to the moon" speech we considered previously include "new", "go", "space", and "moon". If we were to tokenize the text as bi-grams (word pairs), the most common bi-gram in the speech is "the moon". From this information, we can easily surmise that the text is primarily concerned with space travel and going to the moon.

Semantic language models
As the state of the art for NLP has advanced, the ability to train models that encapsulate the semantic relationship between tokens has led to the emergence of powerful language models. At the heart of these models is the encoding of language tokens as vectors (multi-valued arrays of numbers) known as embeddings.

### Get started with text analysis

Azure AI Language is a part of the Azure AI services offerings that can perform advanced natural language processing over unstructured text. Azure AI Language's text analysis features include:

**Named entity recognition** identifies people, places, events, and more. This feature can also be customized to extract custom categories.

**Entity linking** identifies known entities together with a link to Wikipedia.

**Personal identifying information (PII)** detection identifies personally sensitive information, including personal health information (PHI).

**Language detection** identifies the language of the text and returns a language code such as "en" for English.

**Sentiment analysis** and opinion mining identifies whether text is positive or negative.

**Summarization** summarizes text by identifying the most important information.

**Key phrase extraction** lists the main concepts from unstructured text.

##### Link

https://learn.microsoft.com/en-us/azure/cognitive-services/text-analytics/overview

## Understand question answering

Question answering supports natural language AI workloads that require an automated conversational element. Typically, question answering is used to build bot applications that respond to customer queries. Question answering capabilities can respond immediately, answer concerns accurately, and interact with users in a natural multi-turned way. Bots can be implemented on a range of platforms, such as a web site or a social media platform.

## Conversational language understanding

To work with conversational language understanding (CLU), you need to take into account three core concepts: utterances, entities, and intents.
Utterances
An utterance is an example of something a user might say, and which your application must interpret. For example, when using a home automation system, a user might use the following utterances:

"Switch the fan on."

"Turn on the light."

Entities
An entity is an item to which an utterance refers. For example, fan and light in the following utterances:

"Switch the fan on."

"Turn on the light."

Intents
An intent represents the purpose, or goal, expressed in a user's utterance. For example, for both of the previously considered utterances, the intent is to turn a device on; so in your CLU application, you might define a TurnOn intent that is related to these utterances.

### Get started with conversational language understanding in Azure

Authoring
After you've created an authoring resource, you can use it to train a CLU model. To train a model, start by defining the entities and intents that your application will predict as well as utterances for each intent that can be used to train the predictive model.

CLU provides a comprehensive collection of prebuilt domains that include pre-defined intents and entities for common scenarios; which you can use as a starting point for your model. You can also create your own entities and intents.

When you create entities and intents, you can do so in any order. You can create an intent, and select words in the sample utterances you define for it to create entities for them; or you can create the entities ahead of time and then map them to words in utterances as you're creating the intents.

You can write code to define the elements of your model, but in most cases it's easiest to author your model using the Language studio - a web-based interface for creating and managing CLU applications.

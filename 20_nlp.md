# Natural Language Processing (NLP)

NLP is the field of AI that helps computers understand, 
interpret and generate human language — text and speech.

## Why is it hard?
Human language is messy and complex:
- Same sentence can mean different things
- "I saw a man with a telescope" — who had the telescope?
- Idioms — "raining cats and dogs" is not literal
- Same word different meanings — "bank" can mean river 
  bank or financial bank
- Sarcasm, slang, context — all difficult for computers

## Key NLP tasks:

**Text Classification**
Categorizing text into predefined groups.
Example: Spam or not spam.

**Sentiment Analysis**
Determining if text is positive, negative or neutral.
Example: Analyzing customer product reviews.

**Named Entity Recognition (NER)**
Identifying names of people, places, organizations.
Example: "Elon Musk founded Tesla in California"
→ Person: Elon Musk, Organization: Tesla, Place: California

**Machine Translation**
Translating text from one language to another.
Example: Google Translate.

**Text Generation**
Generating new text based on input.
Example: ChatGPT.

**Speech Recognition**
Converting spoken words to text.
Example: Siri, Alexa, Google Assistant.

## Key techniques:

**Tokenization:**
Breaking text into smaller pieces called tokens.
Example: "I love momos" → ["I", "love", "momos"]

**Stop Word Removal:**
Removing common words that don't add meaning.
Example: "the", "is", "and", "a" get removed.

**TF-IDF (Term Frequency — Inverse Document Frequency):**
Converts text into numbers representing word importance.
- TF — how often a word appears in the document
- IDF — how rare the word is across all documents
Common words like "the" get low scores.
Rare meaningful words like "winner" get high scores.
Used in SMS spam classifier project.

**Word Embeddings:**
Representing words as vectors where similar words 
are close together in vector space.
Example: "King" - "Man" + "Woman" ≈ "Queen"

**Transformers:**
Most modern NLP architecture. Powers ChatGPT and BERT.
Understands context — knows "bank" means different 
things in different sentences.

## SMS Spam Classifier pipeline:
1. Tokenization — split emails into words
2. Stop word removal — remove meaningless words
3. TF-IDF — convert words to numbers
4. Naive Bayes — classify based on those numbers

## Advantages:
- Can understand context and meaning
- Works across many languages
- Powers incredible real world applications

## Disadvantages:
- Still struggles with sarcasm and nuance
- Needs huge amounts of data
- Can reflect biases in training data
- Computationally expensive

## Real world examples:
- Gmail spam filter
- Google Translate
- ChatGPT and other chatbots
- Autocomplete on your phone
- Voice assistants
- Sentiment analysis for product reviews

# Introduction
MariTalk is a chatbot that has been specially trained to understand Portuguese well. This repository contains the code and documentation explaining how to use the MariTalk API.

# Usage Example
This Google Colab contains an example showing how to use the API, which is similar to ChatGPT's API:

[Google Colab Example](https://colab.research.google.com/drive/13tieiQdQqYDQGHI8aLtlqoBWMpJ2elyo?usp=sharing)

You can find more details about the API at https://chat.maritaca.ai/docs

# Technical Aspects

MariTalk is based on a Large Language Model specially trained for Portuguese.
It is able to follow instructions in a zero-shot manner, like ChatGPT. 

### Rate Limit
At the moment, there is a limit of 4 requests per minute to ensure that everyone has the opportunity to test the model. If your request is denied due to exceeding this limit, you will receive an HTTP 429 error.

### Maximum sequence length 
Currently, we support a maximum sequence length of 2048 tokens, which is equivalent to approximately 1000 words in Portuguese. We will soon support 8196 tokens.

### Throughput
It takes about 1 to 2 seconds to generate the first token given a sequence of 1000 tokens as input.
After that, new tokens are generated at a rate of 10 to 15 tokens/sec.

## Web Interface
Try the Web interface at:
[chat.maritaca.ai](chat.maritaca.ai)

<img src="imgs/web_interface.png" width="600">

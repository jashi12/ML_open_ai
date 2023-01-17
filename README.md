# File Classifier

This repository contains code for classifying files as suspicious or not using the OpenAI GPT model.

OpenAI API credentials can be gotten from [here](https://beta.openai.com/signup/). This is a proof of concept for a scalable solution to investigating MFT logs of compromised endpoints/servers. 

### Data

The code uses a dataframe of file paths, you can use your own dataset or create a new one. This concept is extremely versatile.

## Built With

* [Python](https://www.python.org/) - The programming language used
* [pandas](https://pandas.pydata.org/) - Data manipulation library
* [openai](https://beta.openai.com/) - API to access GPT model

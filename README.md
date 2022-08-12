# TwitterBot
These scripts are intended to make a Twitter bot with AI generated tweets and other actions handled by an expert system. These scripts were developed to evaluate the ability of AI to attract engagement completely autonomously on Twitter.

TweetPuller
	Intended to be used with the GPT model to generate tweets. GPT provides better results when fine tuned. This script downloads tweets into a clean format to use to fine-tune the GPT model. This script can be run locally on your machine, but you must have a twitter account with developer access to generate the keys.

TweetPusher
	System designed to tweet, retweet, and follow other accounts from the bot account. AI would take a long time to train on actions on twitter so an expert system has been designed with a variety of weights selected to only retweet and tweet during the best times, and to only follow and retweet the most advantageous accounts. Tweets are sent by reading the generated tweets from a csv file. This script can also be run locally on your machine, but you must have a twitter account with developer access to generate the keys.

TweetGenerator_Hivemind_GPT-J_6B
	Essentially the hivemind downscaled GPT-j model with code to generate a resulting csv in a format readable by the tweetpusher. Unless you have the resources locally to fine tune this model, Google Colab is recommended.
	Link for TweetGenerator https://colab.research.google.com/drive/1nVDkXfdec2p-nLU7rMTStF3QWdtx1MdT?usp=sharing
	Link for Original Hivemind Model https://colab.research.google.com/drive/1ft6wQU0BhqG5PRlwgaZJv2VukKKjU4Es?usp=sharing

TweetGenerator_GPT-2
	This model is weaker than the hivemind model, but the code for the model is significantly more accessible thanks to the huggingface libraries. Also generates csv files readable by the tweetpusher
	Link for TweetGenerator https://colab.research.google.com/drive/13BiPER0KHsFlPUspx99bVwlnFk7DOLL9?usp=sharing

Here you'll find all the important reading materials like list of research papers, blogs, algorithm writeups, etc. All the reading material that you'd ever need to do this project have been summarized below. Before starting with the material, we'd like everyone of you to first [watch this video from MLCon](https://www.youtube.com/watch?v=P0jd8AHwjXw&list=WL&index=13&t=2566s)

# A bit of advice before you start reading
To a lot of beginners out there, there'll be a lot of new concepts in the research papers that you might not know. Like one of the research paper uses AutoEncoders neural network. Which is something maybe the experienced ones might not know. That's where your research mindset kicks in. Whenever you are reading a research paper to implement it, it becomes really helpful to google/ChatGPT something that you don't understand. If you come up with autoencoders and don't know what they are, no worries, google it and you'll get tons of free resources to use. Still not able to find the resources, no worries, that's what we mentors are here for. 
***Read the abstract of each paper and then finalize by 14th May which research paper you are going to implement. On 15th of May, we'll be sharing a sheet where you'll have to fill up the name of the research paper that you are going to implement.***
The point is to google up a lot of things to finally understand the paper. 
Understanding a majority of the below written research papers have some pre-requisites:
1. Have an understanding of basic Deep Learning concepts of percpetrons, neural networks like CNN, etc. Some algorithms like **Backprop** would be useful as well. 
2. Understanding of mathematics behind these algorithms, models, neural nets, etc. 
3. Having mathematical understanding of calculus(*you know this from your calculus courses*), linear algebra(*MA106 is more than enough*), and basic stats(*you'll know it alongside the project as you google up things and read the resources provided by us*). 

# Traditional Chess AI
This section is mostly about how traditional chess AI used various hardcoded algorithms alongwith brute-force. 
It's not necessary to read this section, but it'll be quite fun to know how chess engines have become so advanced. You'd appreciate the Deep Learning approach much better if you have even the slightest of idea how older chess engines used to work. So its all on the reader if he wants to read this section or not. 
[A short introduction to some of the chess engines](https://www.cs.cornell.edu/boom/2004sp/ProjectArch/Chess/algorithms.html#quiescence)
[Rune Djurhuus's Slides on Chess engines](https://www.uio.no/studier/emner/matnat/ifi/INF4130/h17/undervisningsmateriale/chess-algorithms-theory-and-practice_ver2017.pdf)

# Deep Learning Chess AI

## DeepChess

[The paper](https://www.cs.tau.ac.il/~wolf/papers/deepchess.pdf)

It's an excellent paper that focusses on using AutoEncoders for building the neural network. The architecture of the neural net is a bit more on the complicated side as it uses hybrid networks. But the paper is fairly simple to understand for anyone who has worked with neural networks before. The implementation of the model might be difficult at first. 

## Maia Chess

[The paper](https://arxiv.org/abs/2006.01855)
[The website](https://maiachess.com/)

This paper focusses more on creating a *human-like* chess AI rather than an AI that plays the best. That's one of a difference. So rather than winning the game (which is obviosuly one of its secondary goals), the paper focusses on creating a chess AI which, on observations, would be indifferent from a human play. 

## Deep Pink

[The blog](https://erikbern.com/2014/11/29/deep-learning-for-chess)

It's not a research paper, but a hobby project by ## [Erik Bernhardsson](https://erikbern.com/ "Home"), who was Spotify's ex-tech Lead and the guy who built Spotify's entire recommendation system. The architecture is very beginner friendly. Just a CNN for feature extraction and that's all. Although, having a knowledge about traditional chess algorithms like **minimax**, **alpha-beta prunning**, etc. might help. You guys can take inspiration from the blog and how its implmented and build something similar. 
If you need help with resources, feel free to ask us!

## AlphaZero & Leela Chess Zero

So here comes the grand daddy of all. AlphaZero is an engineering marvel. It defeats almost all the chess engines out there, and plays like human. You can't distinguish its play with any human. 

[Read this medium article to know about AlphaZero](https://towardsdatascience.com/alphazero-chess-how-it-works-what-sets-it-apart-and-what-it-can-tell-us-4ab3d2d08867#:~:text=In%20short%2C%20AlphaZero%20is%20a,the%20rules%20of%20said%20games.)
[An excellent blog by Tim Wheeler](http://tim.hibal.org/blog/alpha-zero-how-and-why-it-works/)

Leela chess zero works on similar fashion as AlphaZero. The difference is just the fact that Leela is open-source. 
[Here's the research paper](https://arxiv.org/abs/1712.01815) which is definintely quite more on the difficult side, the architecture does use some advanced neural nets like **ResNet** and reinforcement learning. 

## Giraffe 

[The paper](https://arxiv.org/abs/1509.01549)

Its a chess engine that uses self-play to discover all its domain-specific knowledge, with minimal hand-crafted knowledge given by the programmer. It's based entirely on Deep Reinforcement Learning. It's able to do feature extraction and pattern recognintion. 

## CharlesChess

[The blog](https://towardsdatascience.com/hacking-chess-with-decision-making-deep-reinforcement-learning-173ed32cf503)

It's not a research paper, but a very promising implementation by Octavio Santiago, a research scientist at Microsoft. The paper implmentation uses **Deep-Q-Networks** and neural nets like **LSTM** to achieve the results. 

## Tuur Vanhoutte's Thesis

[The thesis](https://github.com/zjeffer/howest-thesis)

If you are interested in Reinforcement learning and using it to create a chess AI, well this one is for you. Thesis is around 44 pages, much of which is reflecting on previously done work. It's well explained and is easy to understand if you follow along properly. 

## Final statement:
There are tons of chess AI out there each of which is using a different architecture. You have to choose one of the above to implement by **14th May**. 
We have our own simple strategy to make one more chess AI, possibly of more than 2000 ELO rating. If you are interested in knowing it, feel free to contact us. 

#### About the implementation:
Of all these research papers, it will not be very difficult to find the implementation code. To that matter, we'd not advice you to copy code. Reason is obvious: the hardware. All these research papers are implemented keeping in mind the hardware and training time. Usually scientists train these on super-fast TPUs and GPUs and that too for more than 20 days! You guys are just having your online notebooks and a few hours for the same. So, it'll be better for you to implement these papers in such a way that the training might be done easily on online GPUs in a short amount of time(say 20hrs max). And for that, copying the code won't be beneficial. You can take inspiration from the implementation, but we'd advice you to refrain from doing *copy-paste engineering*.






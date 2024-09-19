# What is computer science?  Score yourself











## what is the brain of a computer?

![ea62a80a1984633b1cf98d4193bb106f.jpeg](https://img-blog.csdnimg.cn/img_convert/ea62a80a1984633b1cf98d4193bb106f.jpeg)

## What is GPU? Name a company
The full English name of the GPU is Graphics Processing Unit.

To make it simple: a GPU is a specialized graphics processing chip that does graphics rendering, numerical analysis, financial analysis, code-breaking, and other mathematical and geometric operations.GPUs can run on various smart terminal devices, such as PCs, workstations, gaming consoles, cell phones, tablets, etc.

The relationship between GPU and graphics card is like that between CPU and motherboard. The former is the heart of the graphics card and the latter is the heart of the motherboard. Some partners will take the GPU and graphics card as a thing there are some differences, the graphics card not only includes the GPU, but there are some video memory, VRM voltage regulator module, MRAM chip, bus, fan, peripheral device interfaces, and so on!

The huge difference in the composition of the structure shows that: the CPU is more balanced, but not suitable for doing a lot of computing; GPU is more suitable for doing a lot of computing.

This is not to say that the GPU is more powerful the GPU is more like a large group of factory assembly line workers, suitable for doing a large number of simple operations, very complex can not get. But simple things are done very fast, much faster than the CPU.

Compared to GPUs, CPUs are more like technologists and can do complex operations, such as logic operations, responding to user requests, network communications, and so on. However because the ALU takes up less space and has fewer cores, it is suitable for doing relatively small amounts of complex operations.

# To summarize
GPUs whether they handle graphics rendering, numerical analysis, or AI reasoning. The underlying logic is all about breaking down extremely heavy math for tasks and simplifying it.

Then, using the mechanism of GPU multi-stream processors, a large number of operations are broken down into small, simple operations that are processed in parallel. We can also think of a GPU as a cluster in which each stream processor is a CPU, which makes it easier to understand.

## Who is the strongest between GPU and CPU?
This is not easy to say, the number of transistors inside a better GPU can exceed the number of CPUs, the CPU's strong point is to do logical operations, and the GPU's strong point is to do math operations and graphics rendering. This is the reason why ChatGPT uses a lot of high-performance graphics cards for AI reasoning.

Next, let's do a simple comparison.

Differences in Architectural Composition

CPU and GPU are both computing processors, and their architectural composition includes three parts: ALU, Control, and Cache.

However, the proportion of the three components is very different.

In the CPU, the cache unit accounts for about 50%, the control unit 25%, and the computing unit 25%;

In the GPU, the cache unit accounts for about 5%, the control unit 5%, and the computing unit 90%.

# What is AI?

Deep Learning Machine learning

GPT

# ML

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/4894702905444439aa8eab09d4edd6fd.png)

Semi-Supervised Learning (SSL) is a class of machine learning methods that learn by combining a small amount of labeled data with a large amount of unlabeled data. Compared with purely supervised learning, semi-supervised learning can make more effective use of unlabeled data when labeled data is scarce, and improve the generalization ability and prediction accuracy of the model. In this paper, we will discuss the basic principles of semi-supervised learning, the core algorithms and their applications in practice, and provide code examples to help readers better understand and master this technique.

## What is semi-supervised learning
Semi-supervised learning is an approach between supervised and unsupervised learning by utilizing both labeled and unlabeled data for training. In many real-world applications, acquiring large amounts of labeled data is costly, while unlabeled data is usually more abundant. Semi-supervised learning methods can be effective in such environments.

## Advantages of semi-supervised learning
Semi-supervised learning has the following advantages over pure supervised learning:

Reducing labeling cost: by utilizing a large amount of unlabeled data, the reliance on labeled data can be significantly reduced, thus reducing the data labeling cost.
Improve model performance: In the case of scarce labeled data, the generalization ability and prediction accuracy of the model can be improved by introducing unlabeled data.
Better use of data: Make full use of existing unlabeled data to avoid data waste and improve the overall performance of the model.

## 4 Typical Deep Learning Algorithms

Convolutional Neural Network - CNN  https://easyai.tech/en/ai-definition/cnn/
Value of CNN:

![image-20240904161924530](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240904161924530.png)

Able to effectively downsize a large data size image into a small data size (does not affect the results)
Able to retain the features of the image, similar to the principle of human vision
Basic principle of CNN:

Convolutional Layer - Main function is to preserve the features of the image.
Pooling layer - Main function is to reduce the dimensionality of the data, which can effectively avoid overfitting.
Fully connected layer - outputs the results we want according to the different tasks.
Practical applications of CNN:

Image classification, retrieval
Target localization detection
Target segmentation
Face recognition
Bone Recognition
Learn more about Convolutional Neural Networks - CNN (Fundamentals + Unique Value + Practical Applications) in one article.

Recurrent Neural Network - RNN
RNN is an algorithm that can efficiently process sequential data. For example: article content, voice audio, stock price trends...

The reason why it can process sequential data is that the inputs in the front of the sequence also affect the outputs in the back, which is equivalent to having a “memory function”. However, RNN has a serious short-term memory problem, and long-term data has little effect (even if it is important information).

Therefore, based on RNN, LSTM and GRU and other variants of algorithms appeared. These variants have several main features:

Long-term information can be effectively retained
Important information is selected for retention and unimportant information is “forgotten”.
A few typical applications of RNN are as follows:

Text generation
Speech recognition
Machine translation
Image description generation
Video labeling
Learn more about Recurrent Neural Networks - RNN (Unique Value + Optimization Algorithms + Practical Applications) in One Article

Generating Adversarial Networks - GANs
Suppose a city is in a state of law and order, and soon, there will be countless thieves in that city. Among these thieves, some may be expert burglars and some may be unskilled. Suppose that the city starts to clean up its security, and suddenly launches a 'campaign' against crime, and the police start to resume patrols in the city, and very soon a group of 'unskilled' thieves are caught. The reason why the unskilled thieves were caught was because the police's skills were no longer up to snuff, and it's hard to say what happened to the city's law and order after catching the low-end thieves, but it's clear that the average level of the thieves in the city has greatly improved.

The police began to continue to train themselves in crime solving techniques, and began to catch the thieves who were becoming more and more cunning. As these hardened criminals fell into the net, the police developed a special ability to quickly spot a suspicious person in a crowd of people, so that they could go up to the suspect and eventually arrest him or her; the thieves had a hard time as well, because the police had become so much better at their job, and if they continued to act as sneaky as they used to, they would soon be caught by the police. In order to avoid arrest, the thieves try to act less 'suspicious', while the police are also improving their skills to distinguish the thieves from the innocent general public. With this 'exchange' and 'sparring' between the police and the thieves, the thieves become very cautious and with their high level of stealing skills, they behave exactly like the general public, while the police have developed their 'fiery eyes', and as soon as they spot a suspicious person, they are able to spot them and control them in a timely manner - and in the end, we get both the the strongest thieves and the strongest police.

# GPT LLM

## Yolo

Learn more about “What is Generative Adversarial Network - GAN (Basic Concept + Working Principle)”.

Deep Reinforcement Learning - RL
The idea behind reinforcement learning algorithms is very simple, take a game for example, if a certain strategy can be adopted to achieve a higher score in a game, then that strategy is further 'reinforced' in order to continue to achieve better results. This strategy is very similar to the various 'performance rewards' in everyday life. We often use such strategies to improve our gameplay.

In the game Flappy bird, we need to control the bird by simply clicking to avoid various water pipes and fly as far as possible, because the farther we fly, the higher the reward points we can get.

This is a typical reinforcement learning scenario:

The machine has a well-defined role for the bird - the agent
The bird needs to be controlled to fly farther - the goal
Various pipes need to be dodged throughout the game - the environment
The way to avoid the pipes is to make the bird fly a little harder - the action
The farther you fly, the more points you earn - the reward


The biggest difference between reinforcement learning and supervised or unsupervised learning is that it doesn't require a lot of “data feeding”. Instead, you learn certain skills by trying them on your own.

Learn more: “What is Reinforcement Learning? (Basic Concepts + Application Scenarios + Mainstream Algorithms)”.

Summarize
Deep learning belongs to the category of machine learning, and deep learning can be said to be an upgrade on the basis of traditional neural networks, which is approximately equivalent to neural networks.

Deep learning and traditional machine learning are similar in data preprocessing. The core difference is in the feature extraction link, deep learning by the machine itself to complete the feature extraction, without manual extraction.

Advantages of deep learning:

Strong learning ability
Wide coverage, good adaptability
Data-driven, high upper limit
Good portability
Disadvantages of Deep Learning:

High computational effort, poor portability
High hardware requirements
Complex model design
No “human nature”, easy to have bias
4 typical algorithms for deep learning:

Convolutional Neural Network - CNN
Recurrent Neural Networks - RNNs
Generative Adversarial Networks - GANs
Deep Reinforcement Learning - RL

# Why Python?

Python's strengths in AI mainly include:

1. **Rich libraries and frameworks**:
   - With powerful AI and machine learning libraries such as TensorFlow, PyTorch, scikit-learn and more.

2. **Easy to learn and use**:
   - Simple syntax for rapid development and experimentation.

3. **Active community**:
   - Lots of community support and rich resources to help solve problems as well as access learning materials.

4. **Cross-platform compatibility**:
   - Runs seamlessly on different operating systems.

5. **Good integration**:
   - Efficiently integrates with other languages and tools for building complex AI systems.

These features make Python one of the languages of choice for AI development.

Pandas

Numpy

Torch

Tensorflow

https://technews.acm.org/

https://www.anaconda.com/



10%

20 30



50% 50% A-
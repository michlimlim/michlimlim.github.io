---
title: "Federated Learning—a primer"
date: 2021-05-01T12:10:44-04:00
description: "A quick introduction to the decentralized machine learning technology that's already changing the internet."
images: ["/images/fl1.png"]
type: "post"
---

**_Also posted on Medium [here](https://medium.com/@michlimlim/federated-learning-a-primer-b26375737260)._**

![cover](/images/fl1.png)

It’s already in our [keyboards](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html). It’s coming for our website [cookies](https://github.com/WICG/floc). It’s used in clinical trials to connect [siloed patient data](https://owkin.com/hcc-liver-cancer/). Yet not many technologists have heard of **_federated learning_**. Let’s change that.

Federated learning is a type of machine learning that can train models on data that are not shared by its owners. Instead of sending all the data to a central cluster for (machine learning) model training, the model is trained directly on users’ devices. Only model updates are shared. This unlocks unprecedented benefits in privacy. Internet businesses may stop collecting user data. More excitingly, industries which have long resisted machine learning for privacy and legal reasons — medicine, finance, governance — may now get to utilize machine learning!

Why then is federated learning less buzzed about than its decentralized peer, cryptocurrencies? One reason is that it’s a mouthful to explain. Since presenting my [thesis](https://drive.google.com/file/d/1Lgq_zoJeNW99Qln8HZfFs4bPtAv-eJrI/view) on federated learning two years ago, I’ve found that the best way to explain it is to understand how the data flow differs in the federated case compared to the centralized case.

**Centralized machine learning**

![centralized](/images/fl2.png)

**Today, it is typical to send our sensitive data to corporations in exchange for smarter software.** Take how Facebook makes your newsfeed more engaging. Step 1: By using the Facebook newsfeed, we send our demographic information and clicks to its data centers. Step 2: Facebook trains a model on our aggregated data to figure out what types of people will click on what. It then ranks a news feed based on our personal information. Step 3: It loads us that newsfeed.

You start to see the problem. One hack on the central source happens and our data becomes public. The [NSA](https://www.washingtonpost.com/world/national-security/nsa-infiltrates-links-to-yahoo-google-data-centers-worldwide-snowden-documents-say/2013/10/30/e51d661e-4166-11e3-8b74-d89d714ca4dd_story.html) has been reading our Google information — location data, emails, photos. Someone leaked our [DNA](https://www.bloomberg.com/news/articles/2018-06-05/hack-of-dna-website-exposes-data-from-92-million-user-accounts). The internet is more secure than ever, but the cost of any hack has exploded [as more and more personal information](https://en.wikipedia.org/wiki/2017_Equifax_data_breach) has been aggregated by so many firms. It’s why healthcare providers, financial institutions, and governments prefer their data stay on devices they own. They would rather their data be safely siloed even if it means giving up on machine learning.

**Federated Machine Learning**

Federated learning gets us the best of both worlds. Your data stays on your device the whole time.
![federated](/images/fl3.png)

Step 1: You use Facebook and your device trains a model. Step 2: Your device shares only the model updates to a centralized server to be combined. Step 3: Your device receives the combined model. Step 4: Your device uses the combined model to rank your own newsfeed. With the properly secured aggregation methods, the corporation cannot reverse engineer the model to get your data.

Federated learning delivers the benefits of machine learning without forcing users to compromise their privacy. Like a federation of countries, each with its own autonomy, user’s devices have autonomy over their data. If you’re interested in learning more about players and applications of federated learning, check out [Nicole Williams’ piece](https://numinousxperience.xyz/2020/12/21/federated-learning/). For another primer on federated learning, check out [Google’s comic](https://federated.withgoogle.com/). If you’d like to collaborate, discuss, or share thoughts about federated learning, my DMs and email inbox are open!

In industries like e-commerce, retail, news-group or music apps, recommendation system models are one of the most important aspects in customer retention. Presenting to the users what might interest them most is crucial. Also, identifying the most attractive content, and getting customers hooked to specific contents could result in significant revenues to the company.

Based on various data entities, including user details, interests, trending content, etc. models are built to recommend the most relevant content to customers. Companies like Spotify, Netflix, HBO use sophisticated recommendation systems for video and song recommendations. Targeted marketing is a segment of recommendation systems.

A few years ago, Netflix organized a challenge “Netflix Prize”, where they invited people to build a better recommender system than what they had in return for prize money.

***Deep Reinforcement Learning based Recommender System in Tensorflow***

The implemetation of Deep Reinforcement Learning based Recommender System from the paper [ Deep Reinforcement Learning based Recommendation with Explicit User-Item Interactions Modeling by Liu et al]([url](https://arxiv.org/abs/1810.12027)). Build recommender system with [DDPG]([url](https://arxiv.org/abs/1509.02971)) algorithm. Add state representation module to produce trainable state for RL algorithm from data. This is not the official implementation of the paper.

***Procedure***

Trying to improve performance of RL based recommender system. The report contains the result of Using the actor network with embedding layer, reducing overestimated Q value, using several pretrained embedding and applying PER.

Making new embedding files. Previous one contains the information for entire timelines which can mislead model.

Updating Train and Evaluation part. Currently, I didn't follow the exact same training and evaluation procedure in the paper.

**Usage**

*Training*

The saved model of actor and critic are generated after the training is done.
python train.py

Evalutation
Make sure there exist the saved models in the right directory
Run jupyter notebook and check "evaluation.ipynb"

requirements
tensorflow==2.5.0
scikit-learn==0.23.2
matplotlib==3.3.3

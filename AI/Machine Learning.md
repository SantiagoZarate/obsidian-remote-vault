> Field of study that gives the ability to learn without being explicitly programmed.
> 
> *Arthur Samuel*

In general the more options we give the algorithm to learn the better it will perform.

the two main types of ML are:
- Supervised learning
- Unsupervised learning

from those two the former one is the most used in real-world applications and as shown rapid advancements.

Other types are:
- Recommender systems
- Reinforcement learning

# Supervised learning
Refers to algorithm that learn $X$ to $Y$, or input to output mapping, we feed the algorithm with examples to learn form that includes the right answers, and by right answers we mean correct pair of input $X$ and desired output label $Y$, in this way the algorithm eventually learn and just taking the input alone will give a reasonably output.

e.g

| Input (X)     | Output (Y)      | application         |
| ------------- | --------------- | ------------------- |
| Email         | Spam? (0/1)     | Spam filtering      |
| Audio         | Text transcript | Speech recognition  |
| English       | Spanish         | Machine translation |
| Ad, user info | Click? (0/1)    | Online advertising  |

Once the model has learned from those input/output examples, it should be able to take a brand new input and try to produce the appropriate corresponding $Y$.

## Regression algorithm:
Is a type of a supervised learning algorithm that learns to predict numbers out of infinite possible numbers.

e.g:
We are a salesman and we have the prices of houses mapped to their prices, but they are not sequential, when we have a new house size we can try to predict the house price by using a regression algorithm.

## Classification algorithm.
Predicts a category (it doesn't have to be numeric, e.g. whether a picture is about a cat or a dog. In this case we have limited possible outputs, unlike regression algorithm.

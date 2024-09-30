                                     Adversarial attack on Image Classification Model

Adversarial attack refers to the deliberate modification of input images such that it is perceived differently by the AI model. 
In layman's terms, the attacker is generating optical illusions to confuse the AI.
There are many types of adversarial attacks but in this project, I will be focusing on deliberate image misclassification.
In the case of image misclassification, the attacker only wants the output classification to be inaccurate and he/she does not care what the output is.
Repeated output misclassification will result in an inaccurate image classification model.

In this project, I will using the Fast Gradient Sign Attack(FGSM) as the form of adversarial attack.
Described by Goodfollow et.al in Explaining and Harnessing Adversarial Examples, the FGSM method is designed to attack neural networks by leveraging the way they learn - gradients. A normal neural network model works by minimizing the loss by adjusting the weights based on the backpropogated gradients. How this attack works is that it uses the gradient of the loss w.r.t the input data, then adjusts the input data to maximize the loss, casuing the classification model to be inaccurate.

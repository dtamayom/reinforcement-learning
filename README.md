# Reinforcement Learning
Reinforcement Learning module on Advanced Machine Learning course at Universidad de los Andes.

Students: Daniela Tamayo and Isabella Ramos.          
Tutors: Laura Daza and Catalina Gomez


## Before you begin
We strongly suggest you create a specific conda enironment for this task. 
You will have to ensure that all installed dependencies are compatible, otherwise you will probably have issues while running.
The required dependencies and their corresponding compatible versions are included in the file `requirements.txt`. To create the enfironment and install the requirenments we recomend you to use:

```bash
~$: conda create --name rl python=3.7.4
~$: conda activate rl
~$: conda install pytorch torchvision cudatoolkit=10.1 -c pytorch
~$: pip install -r requirements.txt
```

If you have any questions regarding the assignment or RL overall, you can contact us via email or through slack. Remember that you also have the [presentation](RL.pdf) and the [textbook reference books](https://drive.google.com/drive/folders/1bDjUuXlv1xeuA2hJ1TjyjH6WJmZOPTR9?usp=sharing) at your disposal.

## Tutorial
This tutorial is a simple implementation of [CartPole-v0](https://gym.openai.com/envs/CartPole-v1/), one of the available environments in OpenAI-Gym. It consists of a pole attached to a cart moving along a frictionless track. The goal is to prevent the pole from falling over by controlling the force apllied to the cart. Run the tutorial by using this command: 
```bash
~$: python reinforce.py
```

![image](https://cdn-images-1.medium.com/max/1200/1*oMSg2_mKguAGKy1C64UFlw.gif)

If you want to see your CartPole moving, uncomment lines 109 and 124, then run the code on MobaXterm. If you are not able to see the video, remember that the server has no automatic video display. This is why you need to use a virtual framebuffer such as XServer (which comes with MobaXterm) or XQuartz. You might also need to include the -X or -Y flag before you log in: 
```bash
~$: ssh -X yourusername@10.241.69.140
```
If you have any problems, consult this [troubleshooting guide](https://stackoverflow.com/questions/40195740/how-to-run-openai-gym-render-over-a-server).



## Homework
- (2 points) Explore and understand the code. Change hyperparameters and try to change the Policy class by adding or modifying layers. Show your results in an organized table and discuss them. What do you think lead to your best result? Which changes caused the most variation?
- (1 point) For two of your best results, graph Episodes vs Average Reward. Was the graph what you were expecting? Analyze. 
- (2 points) Try a different environment! Choose between [Acrobot-v1](http://gym.openai.com/envs/Acrobot-v1/) and [MountainCar-v0](http://gym.openai.com/envs/MountainCar-v0/). What changed compared to the previous environment? How well did the agent perform in your chosen environment? 

Mountain Car:

![image](https://user-images.githubusercontent.com/66916962/92253564-45fd7e00-ee95-11ea-909e-8e4550f8fa47.png)

Acrobot:

![image](https://svbtleusercontent.com/93Tx9HUAsokfh8i3ce8wCY0xspap.gif)

Include the script for your best result on CartPole and your working code for the alternative environment. 

##Bonus:
Investigate about RL environment packages other than OpenAI-Gym. How might they be useful for different tasks?

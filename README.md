# Reinforcement Learning
Reinforcement Learning module on Advanced Machine Learning course at Universidad de los Andes.

Students: Daniela Tamayo and Isabella Ramos.
Tutor: Laura Daza and Catalina Gomez


## Before you begin
We strongly suggest you create a specific conda enironment for this task. 
You will have to ensure that all installed dependencies are compatible, otherwise you will probably have issues while running.
The required dependencies and their corresponding compatible versions are included in the file `requirements.txt`. To create the enfironment and install the requirenments we recomend you to use:

```bash
~$: `conda create --name rl python=3.7.4`
~$: `conda activate rl`
~$: `conda install pytorch torchvision cudatoolkit=10.1 -c pytorch`
~$: `pip install -r requirements.txt`.
```

If you have any questions regarding the assignment or RL overall, you can contact us via email or through slack. Remember that you also have the [presentation](RL.pdf) and the [textbook reference books](https://drive.google.com/drive/folders/1bDjUuXlv1xeuA2hJ1TjyjH6WJmZOPTR9?usp=sharing) at your disposal.

## Tutorial
Run the tutorial by using this command: 
```bash
~$: `python reinforce.py`
```
If you want to see your CartPole uncomment lines 109 and 124. Then run the code on MobaXterm.

## Homework
- (2 points) Explore and understand the code. Change hyperparameters and try to change the Policy class by adding or changing layers. Show your results and comment. 
- (2 points) For two of your best results, graph Episodes vs Avrage reward. Was the graph what you were expecting? Analyze. 
- (1 point) Try a different environment, choose between [Acrobot-V1](http://gym.openai.com/envs/Acrobot-v1/) and [MountainCar-V0](http://gym.openai.com/envs/MountainCar-v0/). What changed about the previous environment? How well did the agent performed in your chosen environment? 

Mountain Car:
![image](https://user-images.githubusercontent.com/66916962/92253564-45fd7e00-ee95-11ea-909e-8e4550f8fa47.png)

Acrobot:
![image](https://user-images.githubusercontent.com/66916962/92280025-24fd5300-eebe-11ea-8654-f08541bd0cc3.png)

---
layout: post
title:  Easy RL专栏 Reward Shaping, Imitationg learning
date:   2021-09-04 13:26:30
description: Reward Shaping and Imitationg learning
tags: Robot Reinforcement-Learning Machine-Learning
categories: Easy-RL
---
## Reward Shaping
解决稀疏奖励的三个方向：

**Reward Shaping**

​	需要domain knowledge

​	**curiosity** 好奇心驱动的奖励 加入新的奖励函数**内在好奇心模块**  **特征提取器**

**课程学习Curriculum learning** 

​	从易到难让机器学习

​	通用的方法 **逆向课程生成(Reverse Curriculum Generation)**  从黄金状态反推

**分层强化学习Hierarchical RL**

​	分层强化学习是指将一个复杂的强化学习问题分解成多个小的、简单的子问题，每个子问题都可以单独用马尔可夫决策过程来建模。

## Imitation Learning
**Behavior Cloning，BC**

​	机器会遇到专家未曾演示过的状态，因此只观察专家的行为不够，因此出现**Dataset Aggregation(DAgger)** 

**IRL**

​	机器可以跟环境互动，但是得不到奖励。 IRL是先找到奖励函数，找到以后再用强化学习找出最优演员。

**第三人称视角模仿学习Third Person Imitation Learning**

​	用到了 **domain-adversarial training** 
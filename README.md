# udacity-drlnd-collaboration-competition-project
This repository contains the code that is submitted as project 3 of Udacity's Deep Reinforcement Learning Nanodegree

## Project Overview
In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
This yields a single score for each episode.
The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.

### Folder Structure

## Introduction

## Pre-requisites

This project runs as a Jupyter notebook that is ran in a mini-conda enviroment. The following describes the instructions to run the notebook.

### Installing Unity Hub
Follow the instructions and install the Unity Hub that fits your operating system from https://store.unity.com/download

### Installing Miniconda or Anaconda

Anaconda is a free and open-source distribution of Python and R programming languages for scientific computing, that aims to simplify package management and deployment. Miniconda is a slim-down version of Anaconda with less packages included within the installer. The 2 should work similarly with just a different installer download. And Miniconda might require more manual installation of packages. The instructions for installation is found in https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html#regular-installation and it supports Windows, MacOS and Linux.

### Constructing the Conda environment to run the project

This project specific packages for execution and the versions are locked down to prevent version compatibility issues. A conda environment is constructed to host it so that the host machine is not impacted.

#### Create the Conda environment

Run `conda create --name drlnd-p2 python=3.6` (This is only ran once on every host)

#### Activate the Conda environment

Run `conda activate --name drlnd-p2` (This is ran everytime before activating the Jupyter Notebook server)

#### Install the require Python packages

1. Run `conda install -c conda-forge -c pytorch Pillow matplotlib numpy jupyter pytest docopt pyyaml pytorch pandas scipy ipykernel` to install the following packages:

    - tensorflow
    - protobuf
    - grpcio
    - Pillow
    - matplotlib 
    - numpy
    - jupyter 
    - pytest
    - docopt 
    - pyyaml 
    - pytorch
    - pandas 
    - scipy 
    - ipykernel
2. Run `pip install unityagents` to install Unity Agents

## Environment File Download

If you wish to download the unity environment files please follow the instructions below:

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:

   - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
   - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
   - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
   - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) (version 1) or [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) (version 2) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

## Running the agent

1. Setup and activate the conda environment setup 
2. Open Report.ipynb and set the `workspace` and `env_file_name` according to the runtime
3. Run all cells in the notebook
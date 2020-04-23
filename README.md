# PEARL: Efficient Off-policy Meta-learning via Probabilistic Context Variables

Forked from https://github.com/katerakelly/oyster. Please see original repo for original README.

**Purpose of this fork:** This forks removes dependency from MuJoCo when running non-MuJoCo experiments and compiles all dependencies in a virtual environment, as an alternative to Docker in the original implementation. In future, it is also planned to add other non-MuJoCo environments to evaluate PEARL.

**Usage:** After following the installation procedure below, activate the virtual environment running ```source ~/venv/PEARL/bin/activate``` and run the test experiment ```./test_experiment.sh```.

## Installation

NOTE: This installation procedure was tested on Ubuntu 18.04 LTS and Python 3.6.  

Install _pip_ and _virtualenv_ to handle all Python3 dependencies:  
```sudo apt-get install python3-pip```  
```python3 -m pip install --user virtualenv```  

Create a new virtual environment:  
```python3 -m venv ~/venvs/PEARL```

Clone this repo and go to its folder:  
```git clone https://github.com/viniciusguigo/oyster.git```  
```cd oyster```  

Activate the new environment and install dependencies:  
```source ~/venvs/PEARL/bin/activate```  
```pip install wheel```  
```pip install -r requirements.txt```
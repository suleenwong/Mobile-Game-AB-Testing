# Mobile Game AB test analysis

In this study, we aim to analyze user data for a mobile game. As players progress through the levels of the game, they will occasionally encounter gates that force them to wait a non-trivial amount of time or make an in-app purchase to progress. In addition to driving in-app purchases, these gates serve the important purpose of giving players an enforced break from playing the game, hopefully resulting in that the player's enjoyment of the game being increased and prolonged.

In this study, we analyze an AB test where in the control version the gate is placed at level 30 and in the variant version the gate is placed at level 40. The goal is to analyze the impact of the gate level on player retention.


# Requirements and Installation

**Requirements:**

- pyenv with Python: 3.11.1


**Environment:**

For installing the virtual environment you can either use the Makefile and run make setup in a terminal window within the project folder or install it manually using the following commands:

```zsh
pyenv local 3.11.1
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

# About this repo

In this repository you will find:

- Makefile : file for installation of virtual environment
- requirements.txt : requirements file for installation
- ab_test_analysis.ipynb : Python Jupyter notebook with AB test analysis

# Conclusion

The AB test analysis indicates that there is strong evidence that the 7-day retention rate is higher when the gate is at level 30 than when it is at level 40. 

Therefore, if we want to keep retention high — both 1-day and 7-day retention — we should <strong>not</strong> move the gate from level 30 to level 40.


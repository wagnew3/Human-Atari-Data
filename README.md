# Human-Atari-Data
Human Atari Learning Data

# Requirements
gym, matplotlib, pygame

# Collecting Data
python play_atari --env [Gym Environment Spec] --run [Experiment Number] --save_dir [Save Directory]

Gym environment specs are at https://github.com/openai/gym/blob/master/gym/envs/__init__.py

Close the game window before stopping the python program to ensure all results are saved.

# Accessing Data
rewards, done=pickle.load(open ([Save Directory]+[Gym Envrionment Spec]+'_'+str([Experiment Number])+'.p', "rb" ))

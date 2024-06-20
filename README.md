# MSDpostprocess_paper
scripts used for the paper on MSDpostprocess

## Leave one class out tests
SLT05_paperFigures_LOOclassCV.py: This script holds out each lipid class in turn and trains a model on the remaining data then runs inference on the held out lipid class data.

SLT05_paperFigures_LOOclassCV.sbatch: The slurm job submission script used to run the tests.

options_LOOclassCV.toml: The options file used by MSDpostprocess during the tests.

## instrument cross training tests
SLT05_paperFigures_instrumentCrossTraining.py: This script trains a model on each of three datasets then runs inferece on each dataset in turn.

SLT05_paperFigures_instrumentCrossTraining.sbatch: The slurm job submission script used to run the tests.

options_instrumentCrossTraining.toml: The options file used by MSDpostprocess during the tests.

## training stability tests
SLT05_paperFigures_trainingStability.py: This script trains 32 models on random 80-20 train-test splits of the data to assess how stable the training process is. 

SLT05_paperFigures_trainingStability.sbatch: The slurm job submission script used to run the tests.

options_trainingStability.toml: The options file used by MSDpostprocess during the tests.

## other files
SLT05_paperFigures.py: All figures in the paper were generated by this script.

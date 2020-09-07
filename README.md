# NBASalaryPrediction

0) Recommended but optional step: Create a virtual environment for this project
using venv in Python3 or conda (if you use Anaconda as your Python package
manager).

1) Use your package manager (pip or Anaconda) to install the packages from
requirements.txt
  If using pip, run:
    pip install requirements.txt

  If using Anaconda, run:
    conda install --channel conda-forge --file requirements.txt

2) If you want to perform our procedure from scratch, unzip the
nba-players-stats/ and NBA_SalaryHistory/ files. If you simply want to run the
experiments, unzip Data/

3) Run jupyter-notebook from the NBASalaryPrediction directory.

4) Skip this step if you unzipped Data/. If you didn't, then running all cells
in FormattingData.ipynb will perform basic preprocessing on stats and salary
data, then match salaries to players, outputting everything into Data/, which
would be created if it doesn't exist.

5) Run all cells in PreprocessTrainPipeline.ipynb. This performs oversampling,
transformations, and classification of samples into 10 salary tiers (this
parameter can be adjusted in a cell) and saves fitted models to Models/; all
necessary directories will be created by the code.

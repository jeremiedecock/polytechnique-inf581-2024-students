# Polytechnique INF581 2024

Copyright (c) 2019-2024 Jérémie Decock

<img src="https://raw.githubusercontent.com/jeremiedecock/polytechnique-inf581-2024-students/main/logo.jpg" width="250">

- Github repository: https://github.com/jeremiedecock/polytechnique-inf581-2024-students
- Moodle: https://moodle.polytechnique.fr/course/view.php?id=17108


## Lab sessions

### Lab session 4: Dynamic Programming

- Open in Google Colab (short link): http://www.jdhp.org/inf581/lab4
- Open in Google Colab: 
- Open in MyBinder: 
- Open in NbViewer: 
- Download the notebook file: 

### Lab session 5: TD Learning, QLearning and SARSA

- Open in Google Colab (short link): http://www.jdhp.org/inf581/lab5
- Open in Google Colab: 
- Open in MyBinder: 
- Open in NbViewer: 
- Download the notebook file: 


## Run INF581 notebooks locally in a dedicated Python virtual environment

### Dependencies

C.f. `requirements.txt`

### Installation

#### Posix (Linux, MacOSX, WSL, ...)

From the source code:
```bash
conda deactivate         # Only if you use Anaconda...
python3 -m venv env
source env/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install -r requirements-jupyter.txt
python3 setup.py develop
```

#### Windows

From the source code:
```bash
conda deactivate         # Only if you use Anaconda...
python3 -m venv env
env\Scripts\activate.bat
python3 -m pip install --upgrade pip
python3 -m pip install -r requirements-jupyter.txt
python3 setup.py develop
```

## Run INF581 notebooks locally in a dedicated Docker container

Run Jupyter Lab from Docker:
```bash
docker run -it --rm -p 8888:8888 -v "${PWD}":/home/jovyan/work jdhp/inf581:latest
```
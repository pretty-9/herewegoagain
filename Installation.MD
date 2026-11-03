### 1. Install Python dependencies (Ubuntu/Debian)

```
sudo apt update
sudo apt install python3 python3-pip python3-venv
sudo apt install python3-tk
```

### 2. Create and activate virtual environment

```
mkdir deep-learning
cd deep-learning
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Jupyter and Deep Learning packages

```
pip install notebook ipykernel
pip install numpy pandas matplotlib scikit-learn
pip install tensorflow keras torch torchvision
pip install seaborn
```

For Theano (optional, legacy package):

```
pip install Theano-PyMC
```

Theano may not work with modern Python versions.

### 4. Start Jupyter Notebook

```
jupyter notebook
```

### 5. Verify installation

Run this inside a notebook:

```
import tensorflow as tfimport kerasimport torchprint(tf.__version__)print(keras.__version__)print(torch.__version__)
```

Next time, just run:

```
cd deep-learning
source .venv/bin/activate
jupyter notebook
```

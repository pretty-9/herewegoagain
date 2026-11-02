You can install Jupyter Notebook using Python's package manager, `pip`.

Since you're using Linux, follow these steps.

### Step 1: Check if Python is installed

Open your terminal and run:

```
python3 --version
```

Check pip:

```
pip3 --version
```

If either is missing, on Ubuntu/Debian install them using:

```
sudo apt update
sudo apt install python3 python3-pip python3-venv
```

### Step 2: Create a virtual environment (recommended)

```
mkdir jupyter-work
cd jupyter-work
python3 -m venv .venv
source .venv/bin/activate
```

### Step 3: Install Jupyter Notebook

```
pip install notebook
```

### Step 4: Launch Jupyter Notebook

```
jupyter notebook
```

This will start a local server and normally open Jupyter Notebook in your browser at:

`http://localhost:8888`

### Step 5: Create your first notebook

1. Click New → Python 3 (or use the New Notebook option).
2. Enter Python code in a cell.
3. Press `Shift + Enter` to execute it.

For example:

```
print("Hello, Jupyter Notebook!")
```

### Step 6: Install libraries for Deep Learning

Since you're preparing for your Deep Learning practical exam, you may need:

```
pip install numpy pandas matplotlib scikit-learn tensorflow keras
```

Tip: Whenever you want to use Jupyter again, activate your virtual environment and run `jupyter notebook`. You don't need to reinstall it.

---------------------------------------------------------------------------------------------------------------------------------------------------

1. Install the remaining packages
Open your terminal, activate your virtual environment, and run:

PyTorch:
pip install torch torchvision torchaudio


Theano:

The original Theano is discontinued and may not work with modern Python versions. For studying its functionality, you can try the maintained successor:
pip install Theano-PyMC


However, Theano-PyMC is also an older package and may have compatibility issues.
2. Verify your installations
Open Jupyter Notebook and execute:
import tensorflow as tfimport kerasimport torchprint("TensorFlow:", tf.__version__)print("Keras:", keras.__version__)print("PyTorch:", torch.__version__)



To check Theano separately:
import theanoprint("Theano:", theano.__version__)



If all imports execute without errors, the packages are available in your notebook's Python environment.

<a href="https://www.brainntnu.no"><img src="https://i.imgur.com/S9pM24h.png" width=240 align="right"></a>
# Computer Vision Course

Internkurs i Computer Vision - BRAIN NTNU 2020

## Setup

### Code

1. See course Github-repository: [Computer Vision Course Repository](https://github.com/BRAIN-NTNU/computer-vision-course)
2. Clone repository: `git clone https://github.com/BRAIN-NTNU/computer-vision-course.git`
3. Open cloned directory: `cd computer-vision-course`

### Install Jupyter Notebook

We are using Jupyter Notebook for our course:

<a href="https://jupyter.org/#:~:text=The%20Jupyter%20Notebook%20is%20an,machine%20learning%2C%20and%20much%20more."><img src="https://i.imgur.com/MmxC3mq.png"></a>

Download Jupyter Notebook (official tutorial [here](https://jupyter.org/install.html)):

1. Install with pip: `pip install notebook`
2. Verify successful installation with: `jupyter notebook`
3. End session: Press `cmd`+`C` on Mac, or `ctrl`+`C` on Windows.


### Setup Python environment

We use [`virtualenv`](https://virtualenv.pypa.io/en/latest/index.html) is to manage Python packages for different projects. 
Using virtualenv allows you to avoid installing Python packages globally which could break system tools or other projects. You can also just install the packages specified in the `requirements.txt` globally if you want. Assuming Python 3 already installed. Use `pip` or `pip3` for the commands below, depending on your local environment.

1. Install virtualenv, if not already installed: `pip install virtualenv`
2. Create new environment in `computer-vision-course/`: `virtualenv venv`
3. Activate new environment: `source venv/bin/activate` on Mac, or equivalently `venv\Scripts\activate.bat` on Windows. 
4. Install packages that is needed for course: `pip install -r requirements.txt`
5. Add new virtual environment to Jupyter: `python -m ipykernel install --user --name=venv`.
6. Start jupyter notebook: `jupyter notebook`
7. Open [For Participants]-notebook.
8. Change kernel to `venv`: Select *venv* under *Kernel* > *Change kernel* > *venv*, from the top menu bar

> If you want to remove the virtual environment after the course delete our venv using: `rm -rf venv/` and remove from Jupyter: `jupyter kernelspec uninstall venv`.

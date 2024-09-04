# Urban Computing Lab 1
This repository contains the first assignment for the Urban Computing course in fall 2024. The excersises can be found in _"Lab1_Exercises.ipynb"_. Note that this is merely a warm-up exercise and that it **will not be graded nor does it have to be submitted.**

Before we can work on them we need to set up the environment that we will use during this year's edition of the course. We will use the same method of working throughout the course and that it will make our submission process smoother for later exercises, so make sure to familiarise yourself with it. We will be working in _development containers_ that are completely isolated from your system's OS and software. One of the benefits of this approach is that you won't have to install any languages and dependencies on your machine and that everyone uses the exact same environment. This will benefit reproducibility and allows us to work cross-platform effortlessly.

## Installation
We will be using Visual Studio Code (VS Code) as IDE. The container development functionality of VS Code provides us better reproducibility and will help tremendously in running the code on different machines without effort.

**NOTE: Installing Docker is only possible if you are working on a machine where you have administrator rights.** If you do not have administrator rights, you can work on this notebook via a standard python3 venv environment.

Steps to create our working environment:
- Make sure you have [Docker](https://docs.docker.com/get-docker/) installed on your system.
  - If you are running Linux, make sure to follow the additional post-installation step [Manage Docker as a non-root user](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user).
- Make sure you have [VS Code](https://code.visualstudio.com/) installed on your system. You also might have to resart your PC if you run into permission issues afterwards.
- Clone and open this repository in VS Code.
- Click on the extensions icon in the toolbar: ![Extensions icon](docs/extensions.png).
- Search for the _"Remote Development"_ extension and press the install button ![Install button](docs/install.png).
- (Optional) Search for the _"Docker"_ extension and install this extension. It allows you to manage containers from within VS Code.
- You should now be able to see the _"Open a Remote Window"_ ![Remote Window](docs/remote-window.png) button in the bottom left corner.
- Click this button and select _"Reopen in Container"_.
- The container will now be build, which might take a while for the first time.
- After the container is built, VS Code will be running within the container.
  - You can check if VS Code is running within the container in the bottom left corner. It should say _"Dev Container: Python 3"_.

Your can now open the notebook _"Lab1_Exercises.ipynb"_ and start working on your assignment.

## Tips
- You can install additional Python packages while within the Python container through: `pip install <your package>`.
- A light VS Code theme might be preferred while working with Python notebooks
  - To change themes: File/Code -> Preferences -> Color Theme

## References
### Development Containers
- [Beginner's Series to Dev Containers](https://www.youtube.com/watch?v=61M2takIKl8&list=PLj6YeMhvp2S5G_X6ZyMc8gfXPMFPg3O31) on Youtube

### Numpy & Pandas
- [Cloud X Lab - introduction to Numpy and Pandas](https://cloudxlab.com/blog/numpy-pandas-introduction/)
- [Zero With Dot - Performance of numpy and pandas - comparison](https://zerowithdot.com/python-numpy-and-pandas-performance/)
- [Sofia Heisler - A Beginner’s Guide to Optimizing Pandas Code for Speed](https://engineering.upside.com/a-beginners-guide-to-optimizing-pandas-code-for-speed-c09ef2c6a4d6) basic optimization techniques, see also her PyCon 2017 talk on [YouTube](https://www.youtube.com/watch?v=HN5d490_KKk).
- [Pandas - Enhancing Performance](https://pandas.pydata.org/pandas-docs/stable/user_guide/enhancingperf.html) deeper enhancement techniques
- [Numexpr](https://github.com/pydata/numexpr) easily speed up more complex numpy operations
- [Real Python - Look Ma, No For-Loops: Array Programming With NumPy](https://realpython.com/numpy-array-programming/) a somewhat easier introduction to vectorization
- [Python Like You Mean It - Vectorized Operations](https://www.pythonlikeyoumeanit.com/Module3_IntroducingNumpy/VectorizedOperations.html) a bit more advanced text about vectorization

### Matplotlib
- [Real Python - Python Plotting With Matplotlib (Guide)](https://realpython.com/python-matplotlib-guide/)
- [Practical Business Python - Effectively Using Matplotlib](https://pbpython.com/effective-matplotlib.html)

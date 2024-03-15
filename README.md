TODO:
- Issue realted to starting working directory of Jupyter Notebooks within containers. Check out the [**issue on stack overflow**](https://stackoverflow.com/questions/78159957/how-to-define-the-starting-working-directory-of-a-jupyter-notebook-within-a-vs-c).

# VSCode Dev-Container (Docker) Setup for Data Science Projects

This is a [**containerized dev setup**](https://code.visualstudio.com/docs/devcontainers/containers) respectively related for using [**remote containers**](https://code.visualstudio.com/docs/remote/containers) to work on data science / machine learning problems using **Conda, Git with VSCode**.

The Repo contains a setup of a local development container using docker compose and VS Code to develop data science projects in a consistent and robust but yet in a simple and customisable way. The Repo provides the configurations and installations for your container, so you can straight get started with your data science work while enjoying the benefits of using docker containers.

Find a detailed guide about this VSCode Dev-Container for Data Science on Medium.

**Dev Container Main Configurations and Installations:**
- **Miniconda3**, including Python, Jupyter Notebooks, and more.
    - Using conda to install a pre-defined conda environment.
- **Volume Mapping**: A volume will be used to map a directory on your local file system to a directory inside the Docker container. This way, any changes you make to your code locally will be immediately reflected inside the container, where you can run and test the code.
- **Git:** A distributed version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers who are collaboratively developing source code during software development.
- **VS Code**, including extensions like Python, Jupyter Notebooks, Docker, PyLance and more.

Getting Started:
- Install Docker Desktop
- Install VSCode
- Install VSCode
    - Install VSCode remote container extension: [ms-vscode-remote.remote-containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- Start dev container:  F1 + "Open folder in container ..." 
- Open demo.ipynb or demo.py to try the setup

Optional Steps:
- Change Docker Container in Dockerfile and/or docker-compose.yml
- Add/remove VSCode extensions in .devcontainer/devcontainer.json
- Change Anaconda environment in .devcontainer/environment.yml
- Update gitignore to match your setup
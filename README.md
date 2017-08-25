Docker container to run the `deforestprob` Python package.

The docker comes preinstalled with Debian stretch, Python 2.7, GDAL >=
2.0, Jupyter notebook, and key scientific Python packages to run the
deforestprob Python package.

## Usage

* You can pull the container by running `docker pull ghislainv/docker-deforestprob`.
* Run `docker run -d -p 8888:8888 -v ORIGIN_FOLDER:/home/dockeruser/notebooks ghislainv/docker-deforestprob`
    * Replace `ORIGIN_FOLDER` with a folder on your local machine that you want to persist notebooks in.
* Open your browser and start working with Jupyter notebook.
    * On Linux, the url will be `localhost:8888`.
    * On Windows/OSX, run `docker-machine ip default` (replace `default` with the name of your machine). Then, you'll be able to access Jupyter notebook at `CONTAINER_IP:8888`.

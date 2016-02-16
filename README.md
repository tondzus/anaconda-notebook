# Anaconda-Notebook

Originaly forked from [rothnic/anaconda-notebook](https://github.com/rothnic/anaconda-notebook). Go there to see original README.


### Changes compared to original repo

- uses python2 anaconda instead of python3 one
- installs xgboost
 

### How to use this

1. Clone this repo and `cd` into it's root
2. Build your image with `docker build -t <arbitrary/tag> .`
3. After the image building is done, you can launch your data science virtual env with `docker run -v </host/folder>:</docker/folder> -p 8888:8888 -i -t <your/arbitrary/tag>`.

Personally I use this for kaggle competitions. First I prepare a cometition folder on my system by creating `input` and `scripts` folder and I put all competition data into `input`. Then I share this competition folder with container using `-v` docker option and I use `scripts` folder to store my notebooks.

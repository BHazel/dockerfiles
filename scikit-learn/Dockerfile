FROM python
LABEL maintainer="Benedict W. Hazel <bwhazel@gmail.com>"

RUN apt-get update -y && apt-get upgrade -y \
    && apt-get install -y graphviz \
    && pip install numpy scipy matplotlib ipython scikit-learn pandas pillow mglearn jupyter graphviz

EXPOSE 8888
CMD jupyter notebook --allow-root --ip "*"
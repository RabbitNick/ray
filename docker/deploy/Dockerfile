# The deploy Docker image build a self-contained Ray instance suitable
# for end users.

FROM ray-project/base-deps
ADD ray.tar /ray
ADD git-rev /ray/git-rev
WORKDIR /ray/python
RUN pip install --upgrade pip
#RUN pip install --upgrade setuptools
RUN ls /opt/conda/bin/ 
RUN pip install -e . --verbose
WORKDIR /ray

FROM ubuntu

RUN apt-get update \
        && apt-get install -y \
	python3.6

RUN apt-get update \
        && apt-get install -y \
	python3-pip

RUN apt-get update \
        && apt-get install -y \
	vim

RUN apt-get update \
        && apt-get install -y \
        git


WORKDIR workspace
RUN pip3 install jupyter pandas seaborn numpy
RUN git config --global user.name "myname"
RUN git config --global user.password "password"


EXPOSE 8000
CMD jupyter notebook

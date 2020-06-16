FROM ubuntu

WORKDIR /app

COPY . /app

RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip
    
RUN pip3 install -r requirements.txt

EXPOSE 8866

CMD voila dashboard.ipynb
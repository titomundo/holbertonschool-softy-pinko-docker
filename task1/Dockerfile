FROM ubuntu:latest

RUN apt-get update && apt-get upgrade -y && \
	apt-get install -y python3 python3-pip && \
	rm /usr/lib/python*/EXTERNALLY-MANAGED && \ 
	pip3 install Flask

WORKDIR /app
COPY ./api.py /app/api.py

CMD ["flask", "--app", "api.py", "run", "--host=0.0.0.0", "--port=5252"] 

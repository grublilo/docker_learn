FROM python:3.4 
RUN groupadd -r uwsgi && useradd -r -g uwsgi uwsgi  
RUN pip install Flask uWSGI requests redis
WORKDIR /app
COPY cmd.sh / 
USER uwsgi
CMD ["/cmd.sh"] 

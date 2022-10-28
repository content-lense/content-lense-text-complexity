FROM python:3.10

RUN useradd -m python

USER python

WORKDIR /home/python

COPY requirements.txt ./

RUN pip install -r requirements.txt

COPY ./* ./

EXPOSE 5001

CMD python src/api.py
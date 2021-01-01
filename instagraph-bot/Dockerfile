FROM python:3.7-buster

RUN cd /tmp && git clone https://github.com/simoncrowe/instagraph-bot && pip install --no-cache-dir -r /tmp/instagraph-bot/requirements.txt && rm -r /tmp/instagraph-bot

ENV PYTHONPATH /ig

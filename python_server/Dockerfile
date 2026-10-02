FROM python:3.14@sha256:1ae5b32b33f502335ed9f5ee7afa4387192e9566b1328fc66da836c77c1cfb65

WORKDIR /app
COPY requirements.txt ./
COPY src/ ./src

RUN pip install -r requirements.txt

COPY quotes.txt ./quotes.txt
COPY quotes.txt ./src/quotes.txt
COPY start.sh ./

EXPOSE 8002

CMD ["./start.sh"]

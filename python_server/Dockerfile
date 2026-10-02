FROM python:3.11@sha256:50ffeeb3884b139e654d2ce95300cf67d016febfb93d54ecf68a00d723fa6fc6

WORKDIR /app
COPY requirements.txt ./
COPY src/ ./src

RUN pip install -r requirements.txt

COPY quotes.txt ./quotes.txt
COPY quotes.txt ./src/quotes.txt
COPY start.sh ./

EXPOSE 8002

CMD ["./start.sh"]

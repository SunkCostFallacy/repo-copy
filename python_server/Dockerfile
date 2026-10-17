FROM python:3.15@sha256:e748956ccf3f50c9555f236753bbcd5f430d3937e665d3bd6922dd0e6e591a24

WORKDIR /app
COPY requirements.txt ./
COPY src/ ./src

RUN pip install -r requirements.txt

COPY quotes.txt ./quotes.txt
COPY quotes.txt ./src/quotes.txt
COPY start.sh ./

EXPOSE 8002

CMD ["./start.sh"]

FROM python:3.14@sha256:a2e9788143507cacbb754fcc06ad3b7108ca9c334f97a466906103846107cdd5

WORKDIR /app
COPY requirements.txt ./
COPY src/ ./src

RUN pip install -r requirements.txt

COPY quotes.txt ./quotes.txt
COPY quotes.txt ./src/quotes.txt
COPY start.sh ./

EXPOSE 8002

CMD ["./start.sh"]

FROM python:3.11@sha256:3d39409d0b663c788775e81c4640e376604ec50687d2f5aac7c7b44b32bea79f

WORKDIR /app
COPY requirements.txt ./
COPY src/ ./src

RUN pip install -r requirements.txt

COPY quotes.txt ./quotes.txt
COPY quotes.txt ./src/quotes.txt
COPY start.sh ./

EXPOSE 8002

CMD ["./start.sh"]

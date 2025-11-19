FROM python:3.9-slim

COPY secret.txt /challenge/secret.txt

RUN echo '{"flag": "picoCTF{f0und_th3_s3cr3t_18739}"}' > /challenge/metadata.json

CMD ["tail", "-f", "/dev/null"]

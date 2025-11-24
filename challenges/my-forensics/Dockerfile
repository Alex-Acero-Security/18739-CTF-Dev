FROM python:3.9-slim

COPY capture.pcap /challenge/capture.pcap

RUN tar czvf /challenge/artifacts.tar.gz -C /challenge capture.pcap && \
    echo '{"flag": "flag{Two_S7aGE_dN5_to_ht7P}"}' > /challenge/metadata.json  
    

CMD ["tail", "-f", "/dev/null"]

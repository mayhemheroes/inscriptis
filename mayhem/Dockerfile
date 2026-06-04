FROM python:3.11-bullseye
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y clang
RUN pip3 install atheris

COPY . /inscriptis
WORKDIR /inscriptis
RUN python3 -m pip install . && chmod +x fuzz/inscriptis_fuzz.py

ENTRYPOINT [ ]
CMD ["/inscriptis/fuzz/inscriptis_fuzz.py"]

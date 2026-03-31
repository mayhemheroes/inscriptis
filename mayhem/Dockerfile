FROM python:3.8-bullseye
RUN pip3 install atheris

COPY . /inscriptis
WORKDIR /inscriptis
RUN python3 -m pip install -r requirements.txt && python3 -m pip install . && chmod +x fuzz/inscriptis_fuzz.py

ENTRYPOINT [ ]
CMD ["/inscriptis/fuzz/inscriptis_fuzz.py"]
FROM python:3.8-slim

ENV PATH=/root/.local/bin:$PATH

# Install the required stack
RUN pip install --user jupyterlab \
    pandas \
    numpy \
    matplotlib \
    tensorflow==2.4.1

EXPOSE 8888

CMD [ "/bin/bash", "-c", "jupyter-lab --notebook-dir=/ --ip 0.0.0.0 --no-browser --allow-root"]
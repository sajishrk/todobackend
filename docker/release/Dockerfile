FROM sajish/todobackend-base:latest
MAINTAINER Sajish Krishnan  <sajishrk@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse

FROM alpine:3.8

ADD ./wait-for ./

# PYTHON
RUN apk add --no-cache python py-pip

# CHROME
RUN apk add --no-cache chromium chromium-chromedriver

# ROBOT + LIBRARIES
COPY requirements.txt /tmp/requirements.txt
RUN  pip install -r /tmp/requirements.txt

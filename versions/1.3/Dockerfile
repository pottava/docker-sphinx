# Sphinx v1.3
#
# docker run --rm -v `pwd`/doc:/doc -w /doc pottava/sphinx make html
# docker run --rm -v `pwd`/doc:/doc -w /doc pottava/sphinx /bin/sh -c "make clean && make html"

FROM pottava/python:2.7
RUN apk --no-cache add --virtual build-dependencies py-pip python-dev build-base wget \
      && pip install 'sphinx == 1.3.6' \
      && apk --no-cache add make \
      && apk del build-dependencies

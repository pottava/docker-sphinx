# Sphinx v2.0
#
# docker run --rm pottava/sphinx:2.0
# docker run --rm -v `pwd`:/doc -w /doc pottava/sphinx:2.0 make html
# docker run --rm -v `pwd`:/doc -w /doc pottava/sphinx:2.0 /bin/sh -c "make clean && make html"

FROM pottava/latex:2018

RUN apk --no-cache add python3 py3-pip make
RUN apk --no-cache add --virtual build-deps python-dev build-base \
    && pip3 install 'sphinx == 2.0.1' \
    && pip3 install 'sphinx_rtd_theme == 0.4.3' \
    && find / -depth -type d -name \__pycache__ -exec rm -rf {} \; \
    && apk del --purge -r build-deps

CMD ["sphinx-build", "-h"]

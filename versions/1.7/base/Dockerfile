# Sphinx v1.7
#
# docker run --rm pottava/sphinx:1.7
# docker run --rm -v `pwd`:/doc -w /doc pottava/sphinx:1.7 make html
# docker run --rm -v `pwd`:/doc -w /doc pottava/sphinx:1.7 /bin/sh -c "make clean && make html"

FROM pottava/latex:2017

RUN apk --no-cache add python3 py3-pip
RUN apk --no-cache add --virtual build-deps python-dev build-base \
    && pip3 install 'sphinx == 1.7.2' \
    && pip3 install 'sphinx_rtd_theme == 0.2.5b2' \
    && find / -depth -type d -name \__pycache__ -exec rm -rf {} \; \
    && apk del --purge -r build-deps

CMD ["sphinx-build", "-h"]

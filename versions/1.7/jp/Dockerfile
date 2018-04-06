# Sphinx v1.7 with Japanese
#
# docker run --rm -v `pwd`:/doc -w /doc pottava/sphinx:1.7jp /bin/sh -c "make clean && make latex && cd _build/latex && uplatex -interaction=nonstopmode sample.tex && dvipdfmx sample.dvi"

FROM pottava/sphinx:1.7

RUN tlmgr install collection-langjapanese \
      collection-latexrecommended collection-latexextra

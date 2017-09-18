FROM ocaml/opam:debian-stable_ocaml-4.01.0
LABEL maintainer="Benedict W. Hazel <bwhazel@gmail.com>"

RUN opam install -y core utop \
    && eval `opam config env` \
    && echo '#use "topfind";;' >> ~/.ocamlinit \
    && echo '#thread;;' >> ~/.ocamlinit \
    && echo '#camlp4o;;' >> ~/.ocamlinit \
    && echo '#require "core.top";;' >> ~/.ocamlinit \
    && echo '#require "core.syntax";;' >> ~/.ocamlinit \
    && echo 'open Core.Std;;' >> ~/.ocamlinit

CMD ["utop"]
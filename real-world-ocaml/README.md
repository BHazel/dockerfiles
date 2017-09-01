# Real World OCaml

This image is the base installation required to work with the examples in the **Real World OCaml** book by Y Minsky, A Madhavapeddy and J Hickey available at https://realworldocaml.org.

It is configured with:

* OCaml 4.01.0 (based on stable Debian image with OCaml and OPAM installed and configured)
* utop (configured)
* Core

**Please note:** Additional required packages, as outlined in the [installation instructions](https://github.com/realworldocaml/book/wiki/Installation-Instructions) are not included in this image.

To start a container straight into **utop with Core opened** run:

`docker run -it --rm bwhazel/real-world-ocaml`

Alternatively, to start a container at a shell prompt run:

`docker run -it --rm bwhazel/real-world-ocaml bash`

To work with OCaml files outside of the container attach a volume to the desired location:

`docker run -it --rm -v /path/to/host/directory:/path/in/container bwhazel/real-world-ocaml bash`
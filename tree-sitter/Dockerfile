FROM rust:1.76-buster
RUN apt-get update && apt-get install -y nodejs
RUN cargo install --locked tree-sitter-cli && tree-sitter init-config && mkdir /root/src
WORKDIR /root/src
RUN git clone https://github.com/tree-sitter/tree-sitter-php
CMD ["bash"]

FROM eclipse-temurin:8
RUN apt-get update && apt-get install -y ant git
RUN git clone https://github.com/javacc/javacc
WORKDIR /javacc
RUN ant && echo 'export PATH=$PATH:/javacc/scripts' >> /root/.bashrc
CMD ["bash"]

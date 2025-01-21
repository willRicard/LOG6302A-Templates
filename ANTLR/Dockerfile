FROM eclipse-temurin:11
RUN apt-get update && apt-get install -y maven git
RUN git clone -b master https://github.com/antlr/antlr4
WORKDIR /antlr4
RUN mvn -DskipTests install
RUN echo 'export CLASSPATH=/root/.m2/repository/org/antlr/antlr4/*/antlr4-*-complete.jar' >> /root/.bashrc && \
    echo "alias antlr4='java -cp /root/.m2/repository/org/antlr/antlr4/*/antlr4-*-complete.jar org.antlr.v4.Tool'" >> /root/.bashrc && \
    echo "alias grun='java -cp /root/.m2/repository/org/antlr/antlr4/*/antlr4-*-complete.jar org.antlr.v4.gui.TestRig'" >> /root/.bashrc
CMD ["bash"]

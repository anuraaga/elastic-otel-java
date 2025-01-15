FROM docker.elastic.co/wolfi/chainguard-base:latest@sha256:dd66beec64a7f9b19c6c35a1195153b2b630a55e16ec71949ed5187c5947eea1
ARG JAR_FILE
ARG EXTENSION_JAR_FILE
COPY ${JAR_FILE} /javaagent.jar
COPY ${EXTENSION_JAR_FILE} /extensions/elastic-otel-agentextension.jar 
RUN chmod go+r /javaagent.jar /extensions

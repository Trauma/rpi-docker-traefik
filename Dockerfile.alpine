FROM hypriot/rpi-alpine-scratch:v3.3
ARG VERSION=v1.0.0-beta.804
RUN apk --no-cache --no-progress add ca-certificates \
  && wget https://github.com/containous/traefik/releases/download/${VERSION}/traefik_linux-arm \
  && chmod +x traefik
EXPOSE 80,443
ENTRYPOINT ["/traefik"]
CMD ["--help"]

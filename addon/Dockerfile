ARG BUILD_VERSION
ARG BUILD_ARCH

FROM jrlegg/leaf2mqtt:${BUILD_VERSION} AS build
FROM ghcr.io/hassio-addons/base/${BUILD_ARCH}:stable

COPY --from=build / /
COPY root/ /

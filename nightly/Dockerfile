FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y gpg ca-certificates
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 51F523511C7028C3
RUN echo "deb https://qgis.org/ubuntu-nightly-release focal main" >> /etc/apt/sources.list.d/qgis.list
RUN apt-get update && \
    apt-get install -y --no-install-recommends --no-install-suggests qgis-server && \
    rm -rf /var/lib/apt/lists/*

RUN useradd -m qgis
USER qgis

EXPOSE 8000

CMD ["/usr/bin/qgis_mapserver"]

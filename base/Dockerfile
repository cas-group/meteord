FROM debian:wheezy
MAINTAINER CAS Group LLC

ENV METEORD_DIR /opt/meteord
COPY scripts $METEORD_DIR

COPY scripts/install_binbuild_tools.sh $METEORD_DIR/install_binbuild_tools.sh
COPY scripts/rebuild_npm_modules.sh $METEORD_DIR/rebuild_npm_modules.sh

RUN bash $METEORD_DIR/init.sh
RUN bash $METEORD_DIR/install_binbuild_tools.sh

EXPOSE 80
ENTRYPOINT bash $METEORD_DIR/run_app.sh

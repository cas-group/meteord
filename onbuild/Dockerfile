FROM johnschult/meteord:base
MAINTAINER CAS Group LLC

ONBUILD COPY ./ /app
ONBUILD RUN bash $METEORD_DIR/on_build.sh

FROM node:8.15.1-stretch

LABEL net.quadric.vendor="Quadric ApS" maintainer="Ahmed Magdy <ahmed.magdy@quadric.net>"

ARG METEOR_RELEASE
ENV METEOR_RELEASE ${METEOR_RELEASE:-1.8}

RUN echo "Installing meteor release: ${METEOR_RELEASE}"
RUN curl -sL https://install.meteor.com/?release=${METEOR_RELEASE} | sed s/--progress-bar/-sL/g | /bin/sh

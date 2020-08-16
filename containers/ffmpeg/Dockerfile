FROM chiptune/ffmpeg.rpi:latest

# Maintainer
LABEL Pavel Biriukov <syntheticforms@gmail.com>

RUN apt-get update && apt-get -qy install \
  libraspberrypi-bin && \
  rm -rf /var/lib/apt/lists/*

# Set EntryPoint Script
COPY resources/entrypoint.sh /
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]

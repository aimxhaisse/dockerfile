FROM multiarch/ubuntu-debootstrap:amd64-wily      # arch=amd64
#FROM multiarch/ubuntu-debootstrap:armhf-wily      # arch=armhf
#FROM multiarch/ubuntu-debootstrap:powerpc-wily    # arch=powerpc

RUN apt-get update && apt-get install --no-install-recommends -y -q wget

RUN echo "I'm amd64"                              # arch=amd64
#RUN echo "I'm arhmf"                              # arch=armhf
#RUN echo "I'm powerpc"                            # arch=powerpc

ADD overlay-common  /overlay
ADD overlay-amd64   /overlay                      # arch=amd64
#ADD overlay-armhf   /overlay                      # arch=armhf
#ADD overlay-powerpc /overlay                      # arch=powerpc

CMD ["uname -a; cowsay hello world"]

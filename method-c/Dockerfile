FROM multiarch/ubuntu-debootstrap:amd64-wily      

RUN apt-get update && apt-get install --no-install-recommends -y -q wget

RUN echo "I'm amd64"

ADD overlay-common    /overlay
ADD overlay-amd64   /overlay                      

CMD ["uname -a; cowsay hello world"]

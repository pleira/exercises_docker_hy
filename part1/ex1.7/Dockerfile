FROM ubuntu:16.04 

WORKDIR /mydir 
RUN apt-get update && apt-get install -y curl

COPY getweb.sh . 
RUN chmod +x getweb.sh

CMD /mydir/getweb.sh

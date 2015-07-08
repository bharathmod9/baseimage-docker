#FROM ubuntu:14.04
#MAINTAINER Phusion <info@phusion.nl>
FROM ubuntu:15.04
MAINTAINER Arlo Faria <arlo@remeeting.com>

ENV HOME /root
ADD . /build

RUN /build/prepare.sh && \
	/build/system_services.sh && \
	/build/utilities.sh && \
	/build/cleanup.sh

CMD ["/sbin/my_init"]

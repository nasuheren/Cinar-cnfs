FROM ubuntu:16.04
SHELL ["/bin/bash", "-c"]
ENTRYPOINT ["/sbin/init"]
RUN touch /etc/apt/sources.list.d/cinar.list
RUN echo -e $"deb [trusted=yes] http://192.168.13.173:8080/repos/thirdparty/ amd64/\n\
deb [trusted=yes] http://192.168.13.173:8080/repos/cinar/ amd64/\n\
deb [trusted=yes] http://192.168.13.173:8080/repos/interworking/ amd64/\n\
deb [trusted=yes] http://192.168.13.173:8080/repos/latest/ amd64/" >> /etc/apt/sources.list.d/cinar.list
RUN apt-get update
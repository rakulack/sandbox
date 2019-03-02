FROM centos:7
RUN curl -sL https://rpm.nodesource.com/setup_10.x | bash -
RUN yum install yum install -y nodejs gcc-c++ make
RUN yum install -y epel-release
RUN yum install -y golang
RUN npm install -g codebox
EXPOSE 8000
ENTRYPOINT ["codebox","run","./myworkspace","--open"]
CMD ["-p","80:8000"]

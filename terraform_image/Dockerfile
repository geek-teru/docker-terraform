FROM amazonlinux:latest

RUN yum install -y git unzip findutils
RUN cd /opt && \
    git clone https://github.com/tfutils/tfenv.git 
RUN ln -s /opt/tfenv/bin/tfenv /usr/local/bin/tfenv
RUN tfenv install latest:^1.5
RUN tfenv install latest

RUN tfenv use latest:^1.5
RUN ln -s /opt/tfenv/bin/terraform /usr/local/bin/terraform
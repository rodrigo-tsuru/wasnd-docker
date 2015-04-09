FROM rodrigotsuru/ibmim-docker
MAINTAINER Rodrigo Tsuru "caixapostal@gmail.com"
RUN yum install -y curl
RUN cd /tmp && \
curl -O -L https://googledrive.com/host/0B1TfHhOuw5TLMWw2YkNITVhWWjQ/masterpw.txt && \
curl -O -L https://googledrive.com/host/0B1TfHhOuw5TLMWw2YkNITVhWWjQ/secure.dat
RUN /opt/IBM/InstallationManager/eclipse/tools/imcl input /tmp/install.xml -acceptLicense -showProgress -masterPasswordFile /tmp/masterpw.txt -secureStorageFile /tmp/secure.dat

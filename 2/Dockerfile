FROM openshift/jenkins-2-centos7:v3.11

COPY plugins.txt /opt/openshift/configuration/plugins.txt

# Remove example job and install plugins
RUN rm -rf /opt/openshift/configuration/jobs && \
    /usr/local/bin/install-plugins.sh /opt/openshift/configuration/plugins.txt


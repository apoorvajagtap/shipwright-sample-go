FROM registry.redhat.io/ubi9/ubi:latest
RUN rm -rf /etc/rhsm-host 
RUN yum --enablerepo=codeready-builder-for-rhel-9-x86_64-rpms install \ 
    nss_wrapper \
    uid_wrapper -y && \
    yum clean all -y
RUN ln -s /run/secrets/rhsm /etc/rhsm-host 
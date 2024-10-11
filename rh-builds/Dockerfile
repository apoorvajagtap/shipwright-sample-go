FROM registry.redhat.io/ubi9/ubi:latest
RUN rm -rf /etc/rhsm-host 
RUN yum --enablerepo="ubi-9-appstream-debug-rpms" --enablerepo="ubi-9-appstream-source" --enablerepo="ubi-9-baseos-debug-rpms" --enablerepo="ubi-9-baseos-source" install \ 
    policycoreutils -y && \
    yum clean all -y
RUN ln -s /run/secrets/rhsm /etc/rhsm-host 
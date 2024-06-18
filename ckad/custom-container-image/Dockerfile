FROM fedora

RUN dnf -y update && \
dnf -y install procps-ng iproute openssh-server && \
dnf clean install && \
echo "PermitEmptyPasswords yes" >> /etc/ssh/sshd_config


EXPOSE 22
CMD ["/usr/bin/sshd, "-d"]




#
# Govware Exploits
# Docker Runc Exploit
# Victim Container
#

FROM docker:18.09.1-dind

COPY secret.txt /secret.txt
RUN chmod a=,u=rw /secret.txt

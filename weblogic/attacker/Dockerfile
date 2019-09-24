#
# Govware Exploits
# Oracle WebLogic Server Exploit
# Attacker Container
#

FROM kalilinux/kali-linux-docker

# configure kali repos to use https
RUN apt-get install -y  apt-transport-https ca-certificates
RUN echo "deb https://http.kali.org/kali kali-rolling main contrib non-free" > /etc/apt/sources.list && \
    echo "deb-src https://http.kali.org/kali kali-rolling main contrib non-free" >> /etc/apt/sources.list

# install package dependencies
RUN apt-get update && apt-get install -y \
    metasploit-framework \
    nmap \ 
    && rm -rf /var/lib/apt/lists/*

# configure default container command 
CMD [ "bash" ]

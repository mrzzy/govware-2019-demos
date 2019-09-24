#
# Govware Exploits
# Oracle WebLogic Server Exploit
# Victim Container - Weblogic Server
#

FROM openjdk:7u171-jdk

# setup user to run server
RUN useradd user \
        --home-dir /home/user \
        --create-home
USER user
WORKDIR /home/user
        
# copy weblogic server installer
COPY wls1036_generic.jar ./

# install weblogic server
COPY silent.xml ./ 
RUN java -jar wls1036_generic.jar -mode=silent -silent-xml=silent.xml

# start weblogic server
WORKDIR /home/user/Oracle/Middleware_Home/wlserver_10.3/samples/domains/wl_server
RUN sh setExamplesEnv.sh
CMD sh startWebLogic.sh

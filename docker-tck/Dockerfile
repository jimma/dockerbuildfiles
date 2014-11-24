# Use latest Fedora image as the base
FROM jimma/fedora-java
USER jbossws
RUN mkdir /home/jbossws/JEETCK7
ADD JEETCK7 /home/jbossws/JEETCK7
RUN chown -R jbossws /home/jbossws
ENTRYPOINT ["/bin/bash"]

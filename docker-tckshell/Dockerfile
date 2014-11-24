# Create image tckshell image
FROM jimma/jee7tck
USER jbossws
RUN mkdir /home/jbossws/JEETCK7/tck_shell
ADD tck_shell /home/jbossws/JEETCK7/tck_shell
#ADD build.xml /home/jbossws/JEETCK7/trunk/jee7tck-mods/
RUN chmod uog+wrx /home/jbossws/JEETCK7
USER root
RUN chown -R jbossws /home/jbossws
USER jbossws
ENTRYPOINT ["/home/jbossws/JEETCK7/tck_shell/main.sh"]

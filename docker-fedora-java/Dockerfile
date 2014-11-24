# Use latest Fedora image as the base
FROM fedora
# install jdk7, ant and maven
RUN yum -y install java-1.7.0-openjdk-devel.x86_64 unzip mutt
RUN groupadd -r jbossws -g 433 && useradd -u 431 -r -g jbossws -m -s /sbin/nologin -c "jbossws user" jbossws
USER jbossws
RUN cd /home/jbossws && curl -O http://mirrors.cnnic.cn/apache//ant/binaries/apache-ant-1.9.4-bin.tar.gz && tar zxf apache-ant-1.9.4-bin.tar.gz &&  curl -O http://mirrors.cnnic.cn/apache/maven/maven-3/3.2.3/binaries/apache-maven-3.2.3-bin.tar.gz && tar zxf apache-maven-3.2.3-bin.tar.gz
RUN chown -R jbossws /home/jbossws




sudo wget http://www.sonatype.org/downloads/nexus-latest-bundle.zip
sudo chmod 777 nexus-2.11.4-01-bundle.zip
sudo unzip nexus-2.11.4-01-bundle.zip
cd nexus-2.11.4-01/bin
sudo RUN_AS_USER=root ./nexus start


Config nexus on Maven


sudo vim $M2_HOME/conf/settings.xml
    <server>
      <id>nexus</id>
      <username>admin</username>
      <password>admin123</password>
    </server>

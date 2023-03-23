creating jfrog artifact for springpetclinic
-------------------------------------------
* manual steps
```
git clone https://github.com/spring-projects/spring-petclinic.git
sudo apt update
sudo apt install openjdk-17-jdk -y
cd spring-petclinic/
mvn clean package
cd
cd .m2/
vi settings.xml
cd spring-petclinic/
mvn clean install
vi pom.xml
mvn clean install
mvn deploy
```
* maven installation [referhere](https://phoenixnap.com/kb/install-maven-on-ubuntu)
* to view the artifactory [referhere](https://kiranteja.jfrog.io/ui/repos/tree/General/libs-snapshot-local/org)
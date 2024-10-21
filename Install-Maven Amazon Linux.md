
   1.sudo dnf update
   2.sudo dnf install java-11-amazon-corretto
   3.java --version
   4. cd /opt/
   5.ll -a
   6.sudo wget <copy url maven>
   7.sudo tar -zxvf apache-maven-3.9.9-bin.tar.gz
   8.ll
   9.sudo mv apache-maven-3.9.9 /maven
   10.cd /
   11.ll
   12.sudo mv/maven  /opt
   13.ll
   14.cd /opt/
   15.ll
   16.cd maven/
   17.11
   18.cd bin/
   19.ll
   20.cd /etc/
   21.ll (profile/d)
   22.sudo nano /etc/profile.d/maven.sh (path give in this section)
  
     export JAVA_HOME=/usr/lib/jvm/jre-11
	 export M2_HOME =/opt/maven
	 export MAVEN_HOME=/opt/maven/
	 export PATH ={M2_HOME} /bin:{PATH}
  23. cat /etc/profile.d/maven.sh
 export JAVA_HOME=/usr/lib/jvm/jre-11
	 export M2_HOME =/opt/maven
	 export MAVEN_HOME=/opt/maven/
	 export PATH ={M2_HOME} /bin:{PATH}
	 
    24.sudo chmod +x /etc/profile.d/maven.sh
	25.sudo source /etc/profile.d/maven.sh
	26.mvn --version 

	 

   
   
   

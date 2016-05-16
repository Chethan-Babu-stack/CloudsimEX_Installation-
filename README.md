# CloudsimEX_Installation-
Steps to install Cloudsim and CloudSimEX on windows Platform. 


CLOUDSIM INSTALLATION AND WORKING
INSTALLATION PROCEDURE 
Step1: Install any version of JAVA JDK above jdk7 on Windows Operating System.
Step2: Install Eclipse Java EE IDE for Web Developers of version 4.3.x and above.
Step3: After installing the above two softwares, open Eclipse and find Help on top. Click on Help and open Eclipse MarketPlace. Search for Maven 3.2 in the search box and install it as a plugin.
Step4: Download CloudSim and CloudSimEX packages from the given link.
1.	http://www.nikgrozev.org/2014/06/08/cloudsim-and-cloudsimex-part-1/  
2.	https://github.com/Cloudslab/cloudsim
3.	https://github.com/Cloudslab/CloudSimEx
Step5: Open Eclipse and find File option on top.     
File  New  Other  Maven  MavenProject
Unselect the Default WorkSpace Location and select browse to locate the location of CloudSim. Import the downloaded CloudSim package into Eclipse.
Step6: Repeat the Step5 again, but locate and import CloudSimEX package into Eclipse.

WORKING PROCEDURE
Step1: Create a new maven project by File  New  Project  Maven Project Name the Project.
Step2: After project is created, open its pom.xml file and add the following dependencies inside the section.
<dependencies>

    <dependency>
        <groupId>org.cloudbus.cloudsim</groupId>
        <artifactId>cloudsim</artifactId>
        <version>3.1-SNAPSHOT</version>
    </dependency>

    <dependency>
        <groupId>org.cloudbus</groupId>
        <artifactId>cloudsimex-core</artifactId>
        <version>1.0-SNAPSHOT</version>
    </dependency>
    <dependency>
        <groupId>org.cloudbus</groupId>
        <artifactId>cloudsimex-geolocation</artifactId>
        <version>1.0-SNAPSHOT</version>
    </dependency>

    <dependency>
        <groupId>org.cloudbus</groupId>
        <artifactId>cloudsimex-web</artifactId>
        <version>1.0-SNAPSHOT</version>
    </dependency>

    <dependency>
        <groupId>org.cloudbus</groupId>
        <artifactId>cloudsimex-mapreduce</artifactId>
        <version>1.0-SNAPSHOT</version>
    </dependency>

</dependencies>

Step3: Make sure that Eclipse project is configured to use Java 7. Now you can create a class with a main method in the new project and it can import all CloudSim and CloudSimEx classes.

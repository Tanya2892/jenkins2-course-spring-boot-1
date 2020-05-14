pipeline{
    agen any
    stages{
        stage("package")
            steps{
                 bat label: 'package', script: 'T:/Tanya/Softwares/apache-maven-3.6.3-bin/apache-maven-3.6.3/bin/mvn clean package'
                 }
          }
          stage("archive")
            steps{
                 archiveArtifacts artifacts: 'spring-boot-samples/spring-boot-sample-atmosphere/target/*.jar', followSymlinks: false
                 }
          }
        }

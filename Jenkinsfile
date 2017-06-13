pipeline {
  agent {
    node {
      label 'soa12clab'
    }
    
  }
  stages {
    stage('Print Initiation Message') {
      steps {
        echo 'Initiating the Build Process'
      }
    }
    stage('Compile') {
      steps {
        sh '/opt/oracle/middleware/oracle_common/modules/org.apache.maven_3.2.5/bin/mvn package'
      }
    }
  }
}
pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh './dev/make-distribution.sh --name iganlina-spark --pip --r --tgz  -Phive -Phive-thriftserver -Dhadoop.version=3.2.2 -DskipTests'
      }
    }

  }
}
pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh '''/dev/make-distribution.sh --name iganlina-spark -Dhadoop.version=2.8.5 -DskipTests --pip --r --tgz  -Phive -Phive-thriftserver

'''
      }
    }

  }
}
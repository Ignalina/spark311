pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh '''export MAVEN_OPTS="-Xmx24g -XX:ReservedCodeCacheSize=1g"
./dev/make-distribution.sh --name iganlina-spark --pip --r --tgz  -Phive -Phive-thriftserver -Dhadoop.version=3.2.2 -DskipTests'''
      }
    }

  }
}
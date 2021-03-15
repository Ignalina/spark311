pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh '''mkdir .mvn

echo >> "-Xmx3048m -Xms20240m -XX:MaxPermSize=4096m -Djava.awt.headless=true" > .mvn/jvm.config



./dev/make-distribution.sh --name iganlina-spark --pip --r --tgz  -Phive -Phive-thriftserver -Dhadoop.version=3.2.2 -DskipTests



'''
      }
    }

  }
}
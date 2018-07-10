pipeline {
  agent any

  stages {
    stage('build') {

      steps {
        sh 'javac -d . src/*.java'
        sh 'echo Main-Class: rectangular > MANIFEST.MF'
        sh 'jar -cvmf MANIFEST.MF rectangle.jar *.class'
      }
    }
  }
}  

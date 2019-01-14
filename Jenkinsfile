pipeline {
  agent any
  stages {
    stage('start') {
      steps {
		echo 'hello world'
        sh 'env > env.txt'
        for (String i : readFile('env.txt').split("\r?\n")) {
            println i
		}
      }
    }
  }
}
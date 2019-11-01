pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('--clean repo') { 
            steps { 
               sh 'mvn clean'
            }
        }
        stage('--Test'){
            steps {
                sh 'mvn test'
              
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}

pipeline {

    agent any
    tools {
        maven 'apache-maven-3.6.2' 
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn clean compile" 
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }

          stage('installation stage') {
              steps {
                bat "mvn install"
        }
    }

  }

}



/*

pipeline {
    agent any
    stages {
        stage('Compile Stage') {
            steps {
                withMaven(maven: 'apache-maven-3.6.2') { 
                   sh 'mvn clean compile'
                }
            }
        }
        stage('Testing Stage') {
            steps {
                withMaven(maven: 'apache-maven-3.6.2') { 
                   sh 'mvn test'
                }
            }
        }
        stage('Install Stage') {
            steps {
                withMaven(maven: 'apache-maven-3.6.2') { 
                   sh 'mvn install'
                }
            }
        }
    }
}

*/
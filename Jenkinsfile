pipeline {
    agent any

    tools {
        jdk 'JDK17'
    }

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/rahaneom/Prac6.git'
            }
        }

        stage('Compile Java') {
            steps {
                bat '''
                    javac HelloWorld.java
                '''
            }
        }

        stage('Run Program') {
            steps {
                bat '''
                    java HelloWorld
                '''
            }
        }
    }
}

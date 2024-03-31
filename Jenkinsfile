pipeline {
    agent any
    stages {
        stage("Compile") {
            steps {
                sh "chmod +x -R ${env.WORKSPACE}"
                sh "./gradlew compileJava"
            }
        }
        stage("Unit test") {
            steps {
                sh "./gradlew test"
            }
        }
    }
}

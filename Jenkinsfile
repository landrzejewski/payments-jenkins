pipeline {
    agent {
        label "built-in"
    }
    tools {
        jdk "jdk17"
        maven "current"
    }
    stages {
        stage("Build") {
            steps {
                bat "mvn clean compile package"
            }
        }
        stage("Test") {
            steps {
                bat "mvn test"
            }
        }
    }
}

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
                bat "mvn clean compile packa"
            }
        }
        stage("Test") {
            steps {
                bat "mvn test"
            }
        }
    }
}

pipeline {
    agent any
    parameters {
    choice choices: ['dev', 'prod'], description: 'My environment is', name: 'ENV'
    }
    environment {
        APP_NAME = "java-app"
    }

    stages {

        stage('jenkinsfile') {
            steps {
                var1=100
                println "my value is: ${var1}"
                println "my environment is: ${env.APP_NAME}"
                println "my aparameter is: ${params.ENV}"
            }

        }

    }
}

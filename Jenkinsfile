pipeline {
    agent any

    parameters {
        choice(
            name: 'ENV',
            choices: ['dev', 'prod'],
            description: 'My environment is'
        )
    }

    environment {
        APP_NAME = "java-app"
    }

    stages {
        stage('jenkinsfile') {
            steps {
                script {
                    def var1 = 100

                     println "my value is: ${var1}"
                     println "my environment is: ${env.APP_NAME}"
                     println "my parameter is: ${params.ENV}"
                }
            }
        }
    }
}

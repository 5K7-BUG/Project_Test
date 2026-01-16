@Library('shared-lib@feature') _

pipeline {
    agent any
    parameters {
        choice(name: 'ENV', choices: ['dev', 'qa', 'prod'])
        }
    stages {
        stage('Deploy') {
            steps {
                deployApp('payment', params.ENV)
            }
        }
    }
}

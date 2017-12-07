#!/usr/bin/env groovy

    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Demo-Project5835/demo2']
    pipelineTriggers([upstream(threshold:'SUCCESS',
    upstreamProjects:'https://github.com/Demo-Project5835/demo')
    ])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}

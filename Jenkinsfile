#!/bin/env groovy

node {
    deleteDir()
    
    checkout scm
    
    properties([buildDiscarder(logRotator(numToKeepStr: '100'))])
    
    sh 'echo Hello World!'
}

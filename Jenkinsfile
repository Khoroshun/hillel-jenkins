#!/bin/env groovy

node {
    deleteDir()
    
    checkout scm

    files = sh(returnStdout:true, script: 'ls')
    println "list of properties"
    println files

    properties([buildDiscarder(logRotator(numToKeepStr: '100'))])
    
    sh "echo Hello World"
}

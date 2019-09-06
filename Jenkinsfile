#!/usr/bin/env groovy
import hudson.model.*
import hudson.EnvVars
import java.net.URL

node{
    stage('Git Checkout'){
        git 'https://github.com/SrivaniV/DevOpsClassCodes.git'
    }
    stage('Compile Addressbook'){
        withMaven(maven:'mavenJn'){
            sh 'mvn compile'
        }
    }
    stage('package Addressbook'){
        withMaven(maven:'mavenJn'){
            sh 'mvn package'
        }
    }
}

pipeline {
    agent any
    stages {
       stage('compile stage'){
         steps{
           withMaven(maven : 'maven')
            sh 'mvn clean compile'
         }
       }
    }
       stage('test stage'){
         steps{
           withMaven(maven : 'maven')
            sh 'mvn clean test'
         }
       }
       stage('deploy stage'){
         steps{
           withMaven(maven : 'maven')
            sh 'mvn clean install'
         }
       }

}

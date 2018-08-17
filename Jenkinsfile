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
    stages {
       stage('test stage'){
         steps{
           withMaven(maven : 'maven')
            sh 'mvn clean test'
         }
       }
    }
    stages {
       stage('deploy stage'){
         steps{
           withMaven(maven : 'maven')
            sh 'mvn clean install'
         }
       }
    }

}

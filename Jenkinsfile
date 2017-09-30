pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        checkout(
        [$class: 'GitSCM', 
        branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [],
        userRemoteConfigs: [[url: 'https://github.com/YAPPi-incubator/jenkins-example-job']]
        ])
        sh 'cat LICENSE'
      }
    }
  }
}
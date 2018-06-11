pipeline {
  agent any
  stages {
    stage('Git Clone') {
      steps {
        git(url: 'git@gitlab.capensis.fr:vagrant/vagrant-canopsis-demo.git', branch: 'master', credentialsId: 'Capensis-gitlab-token')
      }
    }
  }
  environment {
    vagrant_canopsis_demo = '1'
  }
}
pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        git url: 'https://github.com/msaishwarya37-netizen/ishu.git',
          branch: 'main'
      }
    }
    stage('Run Script'){
      steps {
        sh 'chmod +x script.sh'
        sh './script.sh'
        sh 'python3 script.py'
      }
    }
  }
}

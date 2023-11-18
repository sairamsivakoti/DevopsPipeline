pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'I want to plan my Application Devlopment'
      }
    }

    stage('Code') {
      steps {
        echo 'Devlopment Team perform the App Devlopment'
      }
    }

    stage('Build') {
      steps {
        echo 'Build the Application'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing team performs test activity'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deploy the WAR files'
          }
        }

        stage('Release') {
          steps {
            echo 'Move to Release'
          }
        }

        stage('Operate') {
          steps {
            echo 'Test Application Functionality'
          }
        }

      }
    }

  }
}
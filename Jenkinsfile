def podYaml = """
apiVersion: v1
kind: Pod
spec:
  containers:
  - name: stage-container
    image: alpine
    command:
    - cat
    tty: true
"""

pipeline {
    agent {
        kubernetes {
            yaml podYaml
        }
    }
    stages {
        stage('Stage 1') {
            steps {
                container('stage-container') {
                    sh 'echo Running in Stage 1'
                }
            }
        }
        stage('Stage 2') {
            steps {
                container('stage-container') {
                    sh 'echo Running in Stage 2'
                }
            }
        }
        stage('Stage 3') {
            steps {
                container('stage-container') {
                    sh 'echo Running in Stage 3'
                }
            }
        }
        stage('Stage 4') {
            steps {
                container('stage-container') {
                    sh 'echo Running in Stage 4'
                }
            }
        }
        stage('Stage 5') {
            steps {
                container('stage-container') {
                    sh 'echo Running in Stage 5'
                }
            }
        }
    }
}

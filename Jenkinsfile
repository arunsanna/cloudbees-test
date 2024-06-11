pipeline {
    agent none
    stages {
        stage('Stage 1') {
            agent {
                kubernetes {
                    yaml '''
                    apiVersion: v1
                    kind: Pod
                    spec:
                      containers:
                      - name: alpine
                        image: alpine
                        command:
                        - cat
                        tty: true
                    '''
                }
            }
            steps {
                container('alpine') {
                    script {
                        echo 'Running in Stage 1'
                    }
                }
            }
        }
        stage('Stage 2') {
            agent {
                kubernetes {
                    yaml '''
                    apiVersion: v1
                    kind: Pod
                    spec:
                      containers:
                      - name: alpine
                        image: alpine
                        command:
                        - cat
                        tty: true
                    '''
                }
            }
            steps {
                container('alpine') {
                    script {
                        echo 'Running in Stage 2'
                    }
                }
            }
        }
        stage('Stage 3') {
            agent {
                kubernetes {
                    yaml '''
                    apiVersion: v1
                    kind: Pod
                    spec:
                      containers:
                      - name: alpine
                        image: alpine
                        command:
                        - cat
                        tty: true
                    '''
                }
            }
            steps {
                container('alpine') {
                    script {
                        echo 'Running in Stage 3'
                    }
                }
            }
        }
        stage('Stage 4') {
            agent {
                kubernetes {
                    yaml '''
                    apiVersion: v1
                    kind: Pod
                    spec:
                      containers:
                      - name: alpine
                        image: alpine
                        command:
                        - cat
                        tty: true
                    '''
                }
            }
            steps {
                container('alpine') {
                    script {
                        echo 'Running in Stage 4'
                    }
                }
            }
        }
        stage('Stage 5') {
            agent {
                kubernetes {
                    yaml '''
                    apiVersion: v1
                    kind: Pod
                    spec:
                      containers:
                      - name: alpine
                        image: alpine
                        command:
                        - cat
                        tty: true
                    '''
                }
            }
            steps {
                container('alpine') {
                    script {
                        echo 'Running in Stage 5'
                    }
                }
            }
        }
    }
}

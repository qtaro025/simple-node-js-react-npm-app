pipeline {    
    agent any

    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                nodejs(nodeJSInstallationName: 'Node 18.1.0', configId: '<config-file-provider-id>') {
                    sh 'npm config ls'
                }
            }
        }   

        stage('Test'){
            steps {
                sh 'node test'
            }
        }
    }
}

pipeline {
    agent any
    stages {
        stage('Test-Input1') {
            input {
                message 'Please enter GCP Project ID'
                ok 'Submit Project ID'
                parameters {
                    string(name: 'PROJECT_ID', defaultValue: 'PLEASE ENTER PROJECT ID', description: 'GCP Project ID')
                }
            }
            steps {
                echo "GCP Project id=${PROJECT_ID}"
            }
        }
        stage('Test-Input2'){
            input {
                message 'Please GCE Instance Hostname'
                ok 'Submit Hostname'
                parameters {
                    string(name: 'GCE_HOSTNAME', defaultValue: 'PLEASE ENTER HOSTNAME', description: 'GCE Hostname')
                }
            }
            steps {
                echo "GCE Hostname=${GCE_HOSTNAME}"
            }
        }        
    }
}
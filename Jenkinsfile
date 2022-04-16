pipeline {
    agent any
    stages {
        stage('Test-Input') {
            input {
                message 'Please enter GCP Project ID'
                ok 'Submit Project ID'
                parameters {
                    string(name: 'PROJECT_ID', defaultValue: 'PLEASE ENTER PROJECT ID', description: 'GCP Project ID')
                }
            }
            input {
                message 'Please GCE Instance Hostname'
                ok 'Submit Hostname'
                parameters {
                    string(name: 'GCE_HOSTNAME', defaultValue: 'PLEASE ENTER HOSTNAME', description: 'GCE Hostname')
                }
            }
            steps {
                echo "GCP Project id=${PROJECT_ID}"
                echo "GCE Hostname=${GCE_HOSTNAME}"
            }
        }        
    }
}
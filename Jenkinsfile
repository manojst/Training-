pipeline{
    agent any
    stages{
        stage('SCM Checkout'){
            steps{
                git 'https://gitlab.training.dagility.com/manojkumar_gnanasekaran/training'
            }
        }
        stage('Execute Ansible playbook'){
            steps{
                ansiblePlaybook installation: 'ansible', inventory: 'inventory', playbook: 'playbook.yml'
            }
        }
    }
}

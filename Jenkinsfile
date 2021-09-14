pipeline {
    agent {label 'agent'}
    tools {'org.jenkinsci.plugins.ansible.AnsibleInstallation' 'ansible'}
    stages{
        stage('Execute ansible playbook') {
            steps {
                ansiblePlaybook (
                disableHostKeyChecking: true,
                installation: 'ansible',
                inventory: 'inventory',
                playbook: 'playbook.yml')
            }
        }    
    }
}

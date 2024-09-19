pipeline {
    agent any
    parameters {
        booleanParam(name: 'Refresh',
                    defaultValue: false,
                    description: 'Read Jenkinsfile and exit.')
		    }
    
      stages {

        stage('Run playbook') {
            steps {
                sh '''
                      ansible-playbook -v playbook.yaml
                   '''
            }
        }
    }
}

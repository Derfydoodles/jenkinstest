pipeline {
    agent any
    stages {
        stage('Sample') {
            input {
                message "Should we eat"
                ok "Yes, we should"
                submitter "John,Marcia"
                Parameters {
					string(name: 'Person', defaultvalue: 'Mr Jenkins', description: 'Who shoul i offer food to?')
				}
            }
			steps {
				echo "Hello, ${Person}, It's time to eat"
			}
        }
    }
}
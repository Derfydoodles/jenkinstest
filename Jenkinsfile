pipeline {
    agent any
    stages {
        stage('Sample') {
            input {
                message "Should we eat?"
                ok "Yes, we should."
                submitter "John,Marcia"
                parameters {
					string(name: 'Person', defaultValue: 'Mr Jenkins', description: 'Who should i offer food to?')
				}
            }
			steps {
				echo "Hello, ${Person}, It's time to eat"
			}
        }
    }
}

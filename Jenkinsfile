pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/bhavaniCognizant/jmeter_handsOn_CICD.git'
            }
        }
        stage('Run JMeter Test') {
            steps {
                sh 'jmeter -n -t script.jmx -l result.jtl'
            }
        }
    }
}

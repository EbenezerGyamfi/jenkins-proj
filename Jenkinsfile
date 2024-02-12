pipeline{

agent any
environment{
    RELEASE_DATE=20.04
    JAVA_VERSION='R.5.4'
}
  stages{

        stage('build'){
            agent any
            environment {
                DOCKER_FILE=2.3
            }
            steps{
                echo "Hello from the jenkins file level, your docker file is ${DOCKER_FILE}"
            }
        }
        stage('testing stage'){
            agent any
            environment{
                DEV='in dev mode'
            }
            steps{
                echo "Hello, I am in ${DEV} mode"
                ECHO "JAVA VERSION IS ${JAVA_VERSION}"
            }
        }
    }
}
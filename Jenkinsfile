pipeline{

environment{
    RELEASE_DATE=20.04
}
agent any
    stages{

        stage{
            agent any
            environment {
                DOCKER_FILE=2.3
            }
            steps{
                echo "Hello from the jenkins file level, your docker file is ${DOCKER_FILE}"
            }
        }
        stage{
            agent any
            environment{
                DEV='in dev mode'
            }
            steps{
                echo "Hello, I am in ${DEV} mode"
            }
        }
    }
}
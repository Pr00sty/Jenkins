pipeline {
    agent any
    stages {
        stage("PullGitRepo") {
            steps {
                echo "PullGitRepo"
            }
        }
        stage("Tests") {
            parallel {
                stage("UnitTests") {
                    steps {
                        echo "UnitTests"
                    }
                }
                stage("FunctionalTests") {
                    steps {
                        echo "FunctionalTests"
                    }
                }
            }
        }
    }
}

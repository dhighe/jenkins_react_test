
pipeline {
    agent any
      environment {
        PATH = "C:\\Program Files (x86)\\Git\\usr\\bin;C:\\Program Files (x86)\\Git\\bin;"
        stages {
            stage('Compress') {
                steps {
                    script {

                        zip zipFile: "C:/Users/Link-Donald/Documents/Jenkins_Testing/jenkins_react_test.zip", archive: false, dir: "C:/Program Files (x86)/Jenkins/workspace/jenkins_react_test_master"
                    }
                }
            }
            stage('Execute') {
                steps {
                    sh "C:/Users/Link-Donald/Documents/simple.sh"
                }
            }
        }
    }
}






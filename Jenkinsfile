
pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                script {
                    // writeFile file: "C:/Users/Link-Donald/Documents/Javascript/new_file.txt", text: "Some Text"
                    // //...
                    // String fileText = readFile file: "C:/Users/Link-Donald/Documents/Javascript/new_file.txt"

                    zip zipFile: "C:/Users/Link-Donald/Documents/Jenkins Testing/jenkins_react_test.zip", archive: false, dir: "C:/Program Files (x86)/Jenkins/workspace/jenkins_react_test_master"
                }
            }
        }
        stage('Finalize') {
            steps {
                sh "C:/Users/Link-Donald/Documents/simple.sh"
            }
        }
    }
}







pipeline {
    agent any

    stages {
        stage('zip') {
            steps {
                script {
                    rm -r "C:/Users/Link-Donald/Documents/Jenkins_Testing/*"

                    zip zipFile: "C:/Users/Link-Donald/Documents/Jenkins_Testing/jenkins_react_test.zip", archive: false, dir: "C:/Program Files (x86)/Jenkins/workspace/jenkins_react_test_master"
                }
            }
        }
        // stage('Execute') {
        //     steps {
        //         dir ('C:/Users/Link-Donald/Documents/') { 
        //             sh('simple.sh')
        //         }
        //         // bash "C:/Users/Link-Donald/Documents/simple.sh"
        //     }
        // }
    }
}





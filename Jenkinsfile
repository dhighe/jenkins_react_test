
pipeline {
    agent any

    stages {
        stage('clean') {
            steps {
                script {

                    // find 'C:/Users/Link-Donald/Documents/Jenkins_Testing/' -type f -exec rm {} \;
                    rm -r {'C:/Users/Link-Donald/Documents/Jenkins_Testing/*'}

               }
            }
        }

        stage('zip') {
            steps {
                script {
                    
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





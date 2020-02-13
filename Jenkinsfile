/*
pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    environment {
        CI = 'true'
    }
    node {
        stage "Create build output"
        
        // Make the output directory.
        sh "mkdir -p output"

        // Write an useful file, which is needed to be archived.
        writeFile file: "output/usefulfile.txt", text: "This file is useful, need to archive it."

        // Write an useless file, which is not needed to be archived.
        writeFile file: "output/uselessfile.md", text: "This file is useless, no need to archive it."

        stage "Archive build output"
        
        // Archive the build output artifacts.
        archiveArtifacts artifacts: 'output/*.txt', excludes: 'output/*.md'
    }
}


node {

   stage('Test'){
    
    // Make the output directory.
    sh "mkdir -p output"

    // Write an useful file, which is needed to be archived.
    writeFile file: "output/usefulfile.txt", text: "This file is useful, need to archive it."

    // Write an useless file, which is not needed to be archived.
    writeFile file: "output/uselessfile.md", text: "This file is useless, no need to archive it."

    stage "Archive build output"
    
    // Archive the build output artifacts.
    archiveArtifacts artifacts: 'output/*.txt', excludes: 'output/*.md'
 
   }
}

*/

pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                script {
                    // writeFile file: "C:/Users/Link-Donald/Documents/Javascript/new_file.txt", text: "Some Text"
                    // //...
                    // String fileText = readFile file: "C:/Users/Link-Donald/Documents/Javascript/new_file.txt"

                    zip zipFile: "C:/Users/Link-Donald/Documents/Javascript/test.zip", archive: false, dir: "C:/Users/Link-Donald/Documents/Javascript/test"
                }
            }
        }
    }
}

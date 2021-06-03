pipeline {
    agent any
    stages {
        stage("build") { 
            steps { 
                sh "docker build -t hello_there ."
            }
        }
        stage("run") { 
            steps {  
                sh "docker run -rm -d -p 8888:80  --rm hello_there"
            }
        }
    }
}

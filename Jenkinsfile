node{
    stage('code checkout'){
    echo 'checking out the code'
    git 'https://github.com/Aniket-Utekar/war-test.git'
    }
    stage('Compile') {
            steps {
                echo 'Compile the source code' 
            }
        }    
    stage('build & test & package'){
        sh 'mvn clean package'
    }
    
    stage('deploy'){
       deploy adapters: [tomcat9(credentialsId: '37816b2d-fc7d-4acc-b4cd-5a3398736b84', path: '', url: 'http://34.68.99.152:8080/')], contextPath: 'newpath2', war: '**/*.war'
    }
}

node{
    stage ('SCM Checkout'){
        tool name: 'Maven', type: 'maven'
        git 'https://github.com/idigcloud/Jenkins-Pipeline-deploying-Docker-image'

    }
    stage('Compile-Package'){
        sh 'mvn package'
    }
}

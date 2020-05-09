node{
    stage ('SCM Checkout'){
        git 'https://github.com/idigcloud/Jenkins-Pipeline-deploying-Docker-image'

    }
    stage('Compile-Package)'){
        sh 'mvn package'
    }
}

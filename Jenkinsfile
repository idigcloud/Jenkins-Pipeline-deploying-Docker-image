node{
    stage ('SCM Checkout'){
        git 'https://github.com/idigcloud/Jenkins-Pipeline-deploying-Docker-image'
    }
    stage('Compile-Package'){
        def mvnHome = tool name: 'Maven', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }

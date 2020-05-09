node{
    stage ('SCM Checkout'){
         
        git 'https://github.com/idigcloud/Jenkins-Pipeline-deploying-Docker-image'

    }
    stage('Compile-Package'){
        def mvnHome = tool name: 'Maven', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
    stage('Email Notification'){
        mail bcc: '', body: '''Hi Welcome to Jenkins Email Notification Service
Alerts will be received on Jobs

Dwaraka''', cc: 'dwapha@gmail.com', from: '', replyTo: '', subject: 'Jenkins-Job', to: 'idigcloud@gmail.com'
    }
}

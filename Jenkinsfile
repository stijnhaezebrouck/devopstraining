stage('Compile') {
    node ("node1") {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '5ac02c9a-886e-43b1-bc55-24d1af46f632', url: 'https://github.com/stijnhaezebrouck/devopstraining']]])
        sh './gradlew assemble'
    }
}
stage('Test')


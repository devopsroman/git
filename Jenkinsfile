node {  
    stage('Clone sources') {
        git url: 'https://github.com/devopsroman/git.git'
    }
    stage ('Build OMS') {
        sh 'mvn clean install'
    }
    stage ('Upload WAR-file to nexus') {
        sh 'mvn clean deploy'  
    }
}



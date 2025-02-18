pipeline {
    agent any

    stages {
        stage('git checkout') {
            steps {
            git 'https://github.com/kumargaurav039/maven-project.git'
            } }
            stage('build') {
            steps {
            withMaven(globalMavenSettingsConfig: '', jdk: 'JAVA_HOME', maven: 'MVN_HOME', mavenSettingsConfig: '', traceability: true) {
            sh 'mvn build'
}
            }
        }
    }
}


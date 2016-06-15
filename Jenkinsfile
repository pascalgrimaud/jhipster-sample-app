node {
    stage 'checkout'
    checkout scm
    sh "./mvnw clean"

    stage 'npm install'
    sh "npm install"

    stage 'backend tests'
    sh "./mvnw test"

    stage 'frontend tests'
    sh 'gulp test'

    stage 'package'
    sh "./mvnw package -Pprod -DskipTests"
}

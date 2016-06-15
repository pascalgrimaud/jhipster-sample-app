node {
    stage 'checkout'
    checkout scm
    sh "./mvnw clean"

    stage 'backend tests'
    sh "./mvnw test"

    stage 'package'
    sh "./mvnw package -Pprod -DskipTests"
}

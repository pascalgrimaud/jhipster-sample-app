node {
    stage 'checkout'
    checkout scm
    
    stage 'package'
    sh "./mvnw clean package -Pprod"
}

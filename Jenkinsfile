@Library('piper-lib-os') _
node() {
    stages{
        stage('prepare') {
            checkout scm
            setupCommonPipelineEnvironment script:this
        }
        stage('build') {
            mtaBuild script: this
        }
    }
}

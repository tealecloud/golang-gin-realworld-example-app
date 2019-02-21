node {
    stage('Checkout') {
        checkout scm
    }
    stage('Test') {
        sh '/usr/local/go/bin/go test -v ./... -cover'
    }
    stage('Build') {
        sh '/usr/local/go/bin/go build ./...'
    }
    stage('deploy') {
        echo "Deployed"
    }
}

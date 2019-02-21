node {
    stage('Checkout') {
        checkout scm
    }
    stage('Deps'){
        sh '/usr/local/go/bin/go get -v ./...'
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

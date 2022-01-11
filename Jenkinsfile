//import groovy.json.JsonSlurper
pipeline {
    agent any

    stages {
        stage('http-request') {
            steps {
                script{
                    def response = httpRequest url: argUrl,
                    authentication: "httprequest-test"
                    println("status: "+response.status)
                    println("content: "+response.content)
                   
                }
            }
        }
    }
}

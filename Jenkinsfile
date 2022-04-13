node {
    stage('Checkout') { 
        git branch: 'main', 
            url: 'https://github.com/MichaelKim2000/spring-petclinic.git'
    }
    
    stage('Build') {
        //sh './mvnw clean package'
		echo "test jenkins"
        sh 'true'
    }
    
    stage('Results') {
        junit '**/target/surefire-reports/*.xml'
        archiveArtifacts 'target/*.jar'
    }
}
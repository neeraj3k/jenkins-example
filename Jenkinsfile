pipeline {
    agent 
    {
        node{
        label "built-in"
        }
    }
    stages {
        stage ('Compile Stage') {

            steps {
                
                    sh 'mvn clean compile'
                }
            
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mvn test'
                }
            
        }


        stage ('Deployment Stage') {
            steps {
                
                    sh 'mvn install'
                }
            
        }
    }
}

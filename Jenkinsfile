pipeline {

    agent any

        stages {

        stage('Build')    {

            agent {docker {image 'maven:3.3.3'}}

            steps {sh 'mvn -B -DskipTests=true clean package'}
        }

        stage('Test')    {

            agent {docker {image 'maven:3.3.3'}}

            steps {sh 'mvn test'}
        }








    }

}


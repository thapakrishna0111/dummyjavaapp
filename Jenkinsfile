pipeline{
  agent any
    stages{
      stage('Git Checkout'){
        steps{
         git branch: 'main', url: 'https://github.com/thapakrishna0111/dummyjavaapp.git'
        }

      }
      stage('Unit Testing'){
        steps{
	  sh 'mvn clean test'
        } 
      }
       stage('Integration Testing'){
        steps{
           sh 'mvn verify -DskipUnitTests'
        }
      }


    }   
}

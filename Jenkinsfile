pipeline{
  agent any
    stages{
      stage('Git Checkout'){
        steps{
         git branch: 'main', url: 'https://github.com/thapakrishna0111/dummyjavaapp.git'
        }

      }
      stage('Maven Unit Testing'){
        steps{
	  sh 'mvn test'
        } 
      }

    }   
}

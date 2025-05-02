pipeline {
 agent any
 stages {
 stage('Build') {
 steps {
 echo 'Building...'
 // Comandos para compilar el código
  sh 'mvn clean install'
 }
 }
 stage('Test') {
 steps {
 echo 'Testing...'
 // Comandos para ejecutar pruebas
  sh 'mvn test'
 }
 }
 stage('Deploy') {
 steps {
 echo 'Deploying...'
 // Comandos para desplegar el software
  sh 'docker build -t myapp .'
 sh 'docker run -d -p 8080:8080 myapp'
 }
 }
 }
}

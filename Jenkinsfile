pipeline {
 agent any
 stages {
 stage('Build') {
 steps {
 echo 'Building...'
 // Comandos para compilar el código
 sh 'echo "Building..." > build.log'
 sh 'ls -l'
 }
 }
 stage('Test') {
 steps {
 echo 'Testing...'
 // Comandos para ejecutar pruebas
 // (ejemplo: verificar la existencia de un archivo)
 sh 'if [ -f "build.log" ]; then echo "Test Passed"; else echo "Test Failed"; exit 1; fi'
 sh 'echo "Test Passed" > test.log'
 }
 }
 stage('Deploy') {
 steps {
 echo 'Deploying...'
 // Comandos para desplegar el software
 sh 'echo "Deployment successful" > deploy.log'
 }
 }
 }
}

pipeline {

agent any

stages {

stage('Clone Repository') {

steps {

git 'https://github.com/suryanp27/simple-app.git'

}

}

stage('Run Tests') {

steps {

echo 'pytest tests/' // Replace 'tests/' with your test directory

}

}

stage('Build Docker Image') {

steps {

echo 'docker build -t simple-app .'

}

}

stage('Deploy') {

steps {

echo 'docker run -d -p 80:80 simple-app'

}

}

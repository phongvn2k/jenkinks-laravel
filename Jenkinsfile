pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/phongvn2k/jenkinks-laravel.git'
            }
        }
        stage('build') {
            steps {
                def laravelDir = '/var/www/jenkins/jenkinks-larave-jenkinks/jenkinks-laravel/'

                dir(laravelDir) {
                    sh 'composer install'
                }
            }
        }
    }
}

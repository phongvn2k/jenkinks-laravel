pipeline {
    agent any
    stages {
        stage('Install Dependencies') {
            steps {
                script {
                    // Đặt đường dẫn đến thư mục Laravel của bạn
                    def laravelDir = '/var/www/jenkins/jenkinks-larave-jenkinks/jenkinks-laravel/'

                    git branch: 'main', url: 'https://github.com/phongvn2k/jenkinks-laravel.git'

                    // Bước này sẽ chuyển đến thư mục Laravel và chạy lệnh composer install
                    dir(laravelDir) {
                        // Chạy lệnh composer install
                        sh 'composer install'
                    }
                }
            }
        }
    }
}


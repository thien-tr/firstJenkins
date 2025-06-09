pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'Build application'
            }
        }
        stage('test') {
            steps {
                echo 'Test application'
                bat """
                    C:\\Users\\Trainer\\AppData\\Local\\Programs\\Python\\Python312\\python.exe F:\\PYTHON\\DEMO\\CICD\\test.py
                """
            }
        }
        stage('deploy') {
            steps {
                echo 'Deploy application'
                 bat """
                    copy "F:\\PYTHON\\DEMO\\CICD\\People.py" F:\\PYTHON\\DEMO\\TEMP_SERVER
                """
            }
        }
    }
}

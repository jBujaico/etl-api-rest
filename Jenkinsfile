pipeline {
    agent any

    stages {
        stage('Clonar repositorio') {
            steps {
                git branch: 'main', url: 'https://github.com/jBujaico/etl-api-rest.git'
            }
        }

        stage('Ejecutar ETL') {
            steps {
                sh 'python transform.py'
            }
        }
    }
}

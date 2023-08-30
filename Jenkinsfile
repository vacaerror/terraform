pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Clonar el repositorio de código fuente
                 script {
                    currentBuild.description = "📥 Checkout code from repository"
                }
               echo 'checkout..'
            }
        }
        
        stage('Build') {
            steps {
                // Compilar tu aplicación (por ejemplo, usando Maven o Gradle)
                 script {
                     currentBuild.description = "🛠️ Building the application"
                }
                echo 'Building'
            }
        }
        
        stage('Deploy') {
            steps {
                // Desplegar tu aplicación en un entorno de prueba
                script {
                    currentBuild.description = "🚀 Deploying the application"
                }
                 
                echo 'Deploy'
            }
        }
        
        stage('Test') {
            steps {
                // Ejecutar pruebas automatizadas (por ejemplo, pruebas de unidad y de integración)
                script {
                    currentBuild.description = "🧪 Running Deploy automated tests"
                } 
                  echo 'Test'
            }
        }
        
        stage('Report') {
            steps {
                // Generar informes de prueba
                 script {
                    currentBuild.description = "📊 Generating test reports"
                }
                echo 'Report'
            }
        }
    }
}

pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        echo 'inicializando'
      }
    }

    stage('Build') {
      steps {
        echo 'contruyendo'
      }
    }

    stage('Test') {
      parallel {
        stage('Integración') {
          steps {
            echo 'intngrando'
          }
        }

        stage('Desempeño') {
          steps {
            echo 'Validando'
          }
        }

      }
    }

    stage('Browser test') {
      parallel {
        stage('Mozila') {
          steps {
            echo 'Fox'
          }
        }

        stage('Chrome') {
          steps {
            echo 'Logo'
          }
        }

        stage('Edge') {
          steps {
            echo 'Spartano'
          }
        }

      }
    }

    stage('Confirmación') {
      steps {
        echo 'Confirmando'
      }
    }

    stage('Analisis estático') {
      steps {
        echo 'Analisando'
      }
    }

    stage('Desplegar') {
      steps {
        echo 'Acción'
      }
    }

  }
}
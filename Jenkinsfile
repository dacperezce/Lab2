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
        stage('Integracion') {
          steps {
            echo 'intngrando'
          }
        }

        stage('Desempeno') {
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

    stage('Confirmacion') {
      steps {
        echo 'Confirmando'
      }
    }

    stage('Analisis estatico') {
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
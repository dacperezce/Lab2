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
        stage('Integraci�n') {
          steps {
            echo 'intngrando'
          }
        }

        stage('Desempe�o') {
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

    stage('Confirmaci�n') {
      steps {
        echo 'Confirmando'
      }
    }

    stage('Analisis est�tico') {
      steps {
        echo 'Analisando'
      }
    }

    stage('Desplegar') {
      steps {
        echo 'Acci�n'
      }
    }

  }
}
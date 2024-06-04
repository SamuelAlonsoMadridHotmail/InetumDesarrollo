pipeline
{
  agent any
  environment
    {
        CIUDAD = "Cieza"
        HABITANTES = 35000
        CLIMA = "Soleado"
    }
  stages
  {
    stage("Información ciudad")
    {
      steps{
        script
        {
          println "Ciudad: ${env.CIUDAD}, Habitantes: ${env.HABITANTES}, Clima: ${env.CLIMA}"
        }
      }
    }
    stage("Comando BAT")
    {
      steps{
        bat 'ipconfig /flushdns'
      }
    }
    stage("Informar usuario")
    {
      steps{
        echo 'El usuario es ${env.username}'
      }
    }
  }
}

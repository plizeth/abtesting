# Request Timer

Aplicacion para hacer peticiones http y tarda en responder el tiempo (en milisegundos) que le indiques por parametros.

## API

#### Http request fixed time
`GET /request-timer/v1/api/timer/fixed/{time}`
  - Description: Peticion http que espera un tiempo fijo pasado por parametro
  - Parameters:
    - time : Tiempo en milisegundos
  - Examples:
    - /request-timer/v1/api/timer/1000

#### Http request with random time
`GET /request-timer/v1/api/timer/rand/{min}/{max}`
  - Description: Peticion http que espera un tiempo aleatorio entre los valores que se pasan por parametro
  - Parameters:
    - min : Tiempo minimo en milisegundos
    - max : Tiempo maximo en milisegundos
  - Examples:
    - /request-timer/v1/api/timer/1000/10000

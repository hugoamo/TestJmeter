# TestJmeter
###  Script Básico de consulta a un API

- Se generan dos casos de prueba positivos

- Para el primer caso solo evaluamos el status code sea igual 202

- Para el segundo caso evaluaremos la respuesta de la peticion


	Feature: Testing a REST API
  El usuario deberia suministrar una solicitud GET a un servicio web,
  opteniendo una repsuesta del codigo del estado
 
  Scenario: Consulta de un API
  
  	Given I Set GET service API
  
  	When I Set request Header
  
 	And send GET HTTPS request
  
 	then I receive valid HTTPS request code 202

# Arquetipo-maven-limpio
Este es un repositorio que contiene la estrucctura inicial para realizar un proyecto spring boot dividido en modulos.

Contenido de los modulos:

	1. application: Contiene todo lo referente a la capa de presentacion. Como son los controladores, en ellos solo se podran inyectar los servicios.
	
	2. domine: Contendra la logica de negocio de la app, si así lo de deseas.
	
	3. dto: Contiene los objectos de tranferencias de datos estos se encontraran accesibles desde varios modulos de la app. Como en application, 
		services, domine entre otros.
	
	4. integration: En este modulo se realizaran las integraciones con los servicios web externos a tu app. 
		Incluye un plugins que auto genera las clases clientes para consumir las funcionalidades expuestas en los wsdl.
	
	5. model: Contiene las definiciones de entidades de la BBDD.
	
	6. repository: Contiene las consultas a la BBDD adicional cuenta con un plugins (QueryDsl) que se puede utilizar para 
		generar las consultas a traves de metodos. https://querydsl.com/static/querydsl/4.4.0/reference/html_single/#intro. 
		
	7. service-api: Contiene la definicion de las interfaces de los servicios a implementar.
	
	8. service-impl: Contiene la implementacion de las interfaces(service-api). Tambien puede tener la definicion de los componentes que convertiran de un model a dto y al contrario.
		Entre otras funcionalidades que requiera la app.
		

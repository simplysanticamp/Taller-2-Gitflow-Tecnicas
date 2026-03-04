# Documento de Pruebas

## 1. Descripcion del Sistema

## 2. Requerimientos a Evaluar

#RF-03 Inscripción a Evento
Un estudiante podrá inscribirse a un evento solo si:
	-	Está registrado. (bolean)
	- El evento tiene cupos disponibles. (bolean)
	- No está previamente inscrito. (bolean)

Si alguna condición no se cumple, el sistema no debe permitir la inscripción.
Un caso valido es:
V,V,F

## 3. Tecnicas de Prueba Aplicadas

#RF-03 Inscripcion a evento:

La tecnica empleada para el FR-03 es la tabla de decicion, empleamos esta tecnica porque el requerimiento nos pide 3 condiciones tales como: estar previamente registrado, cupos disponibles en el evento, tener previamente una inscripcion en el evento, cada uno de estos datos son de tipo bolean lo que hace que sean adecuados para implementarse con dicha tecnica.

## 4. Casos de Prueba Diseñados



## 5. Trazabilidad

## 6. Gestion de Versiones (GitFlow)

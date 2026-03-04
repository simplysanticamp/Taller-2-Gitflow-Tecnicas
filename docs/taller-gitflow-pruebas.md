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

## 4. Casos de Prueba Diseñados

#RF-03 Inscripción a Evento

| Casos | Previamente Registrado | Cupos Disponibles | Inscripción previa | Resultado esperado | Comentario |
| :--- | :---: | :---: | :---: | :---: | :--- |
| 1 | V | V | V | No permitir | Ya está inscrito |
| 2 | V | V | F | Permitir | Cumple todas las condiciones |
| 3 | V | F | V | No permitir | No hay cupos y ya inscrito |
| 4 | V | F | F | No permitir | No hay cupos |
| 5 | F | V | V | No permitir | No está registrado y ya inscrito |
| 6 | F | V | F | No permitir | No está registrado |
| 7 | F | F | V | No permitir | No registrado, sin cupos y ya inscrito |
| 8 | F | F | F | No permitir | No registrado y sin cupos |


## 5. Trazabilidad

## 6. Gestion de Versiones (GitFlow)

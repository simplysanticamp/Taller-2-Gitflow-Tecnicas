# Documento de Pruebas

## 1. Descripcion del Sistema

## 2. Requerimientos a Evaluar
Rf_02-Codido de Estudiante:
 - El código del estudiante debe tener exactamente 8 caracteres. 
 - El código del estudiante debe iniciar con la letra “E”.  
 - Los 7 caracteres restantes deben ser numéricos.  
## 3. Tecnicas de Prueba Aplicadas
- Tecnica aplicada: Partición de equivalencia
- Justificación: Se utiliza Partición de Equivalencia porque el dominio de entrada puede dividirse en clases válidas e inválidas (longitud correcta/incorrecta, prefijo correcto/incorrecto, parte numérica válida/inválida).
## 4. Casos de Prueba Diseñados

| Condición de Entrada | Clases válidas | Clases inválidas |
| :--- | :---: | ---: |
| Longitud de 8 caracteres | 1. E1234567 == 8 Caracteres | 1. E123, < 8 caracteres <br> 2. E12345678910, > 8 caracteres |
| Inicio con la letra "E" | 1. "E"0000000 | 1. "A"9999999 <br> 2. "K"1234567 |
| 7 caracteres restantes <br> deben ser numericos | 1. E1234567 | 2. E123YO08 (Contine caracteres no númericos) <br> 2. E123-#7@ (Contiene caracteres especiales) |

## 5. Trazabilidad



## 6. Gestion de Versiones (GitFlow)

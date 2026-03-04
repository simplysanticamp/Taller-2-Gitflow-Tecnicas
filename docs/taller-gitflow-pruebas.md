# RF-01 Registro de Estudiante (Edad)

## 1. Analisis del requerimiento

## 2. Requerimientos a Evaluar
Rf-01: El sistema debe permitir el registro de estudiantes cuya edad este entre 16 y 65 años inclusive.
Rf-02:
Codido de Estudiante:
 - El código del estudiante debe tener exactamente 8 caracteres. 
 - El código del estudiante debe iniciar con la letra “E”.  
 - Los 7 caracteres restantes deben ser numéricos.  
## 3. Tecnicas de Prueba Aplicadas
RF-01:
Tecnica de prueba unitaria: Analisis de Valor Límite
Justificacion:
El requerimiento define un rango numérico con límites claros (16 y 65).  
Los errores suelen presentarse en los extremos del rango.  
Por ello, el Análisis de Valores Límite es la técnica más adecuada
RF-02:
- Tecnica aplicada: Partición de equivalencia
- Justificación: Se utiliza Partición de Equivalencia porque el dominio de entrada puede dividirse en clases válidas e inválidas (longitud correcta/incorrecta, prefijo correcto/incorrecto, parte numérica válida/inválida).
## 4. Casos de Prueba Diseñados
Rf-01
| ID Caso | Edad Ingresada | Resultado Esperado | 
|---------|----------------|--------------------|
| CP-01   |       16       | Registro permitido | 
| CP-02   |       65       | Registro permitido | 
| CP-03   |       15       | Registro rechazado | 
| CP-04   |       66       | Registro rechazado | 
| CP-05   |       30       | Registro permitido | 
Rf-02
| Condición de Entrada | Clases válidas | Clases inválidas |
| :--- | :---: | ---: |
| Longitud de 8 caracteres | 1. E1234567 == 8 Caracteres | 1. E123, < 8 caracteres <br> 2. E12345678910, > 8 caracteres |
| Inicio con la letra "E" | 1. "E"0000000 | 1. "A"9999999 <br> 2. "K"1234567 |
| 7 caracteres restantes <br> deben ser numericos | 1. E1234567 | 2. E123YO08 (Contine caracteres no númericos) <br> 2. E123-#7@ (Contiene caracteres especiales) |

## 4. Validación de Cobertura

Se probaron ambos límites del rango tambien Se probaron valores al limite de estar fuera del rango  
Se probaron valores inmediatamente dentro del rango.  

## 5. Trazabilidad



## 6. Gestion de Versiones (GitFlow)





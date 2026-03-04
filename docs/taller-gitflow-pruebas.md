# RF-01 Registro de Estudiante (Edad)

## 1. Analisis del requerimiento

El sistema debe permitir el registro de estudiantes cuya edad este entre 16 y 65 años inclusive.

Tecnica de prueba unitaria: Analisis de Valor Límite

Justificacion:
El requerimiento define un rango numérico con límites claros (16 y 65).  
Los errores suelen presentarse en los extremos del rango.  
Por ello, el Análisis de Valores Límite es la técnica más adecuada

###  Casos de Prueba

| ID Caso | Edad Ingresada | Resultado Esperado | 
|---------|----------------|--------------------|
| CP-01   |       16       | Registro permitido | 
| CP-02   |       65       | Registro permitido | 
| CP-03   |       15       | Registro rechazado | 
| CP-04   |       66       | Registro rechazado | 
| CP-05   |       30       | Registro permitido | 

## 4. Validación de Cobertura

Se probaron ambos límites del rango tambien Se probaron valores al limite de estar fuera del rango  
Se probaron valores inmediatamente dentro del rango.  

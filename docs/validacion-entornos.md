# Validación de entornos

## Entorno local
El desarrollador debe comprobar la correcta respuesta del servicio levantando el contenedor Docker local y ejecutando las pruebas unitarias integradas.

## Entorno de pruebas
El equipo de QA verificará la estabilidad del servicio en el entorno de Stage antes de habilitar el paso de documentación al pipeline de despliegue final.

## Criterio para considerar la guía lista
La documentación se considera aprobada únicamente cuando ambos entornos (local y pruebas) hayan sido validados sin alertas de conectividad ni errores de compilación.

## Riesgo de validar solo una parte del proceso
Validar de forma parcial o aislada incrementa el riesgo de subir configuraciones corruptas a producción, lo que podría interrumpir la pasarela de pagos del Checkout Service.
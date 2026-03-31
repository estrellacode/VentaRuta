# VentaRuta

Aplicación móvil desarrollada en Flutter para la gestión de ventas en ruta, integrando escáner de códigos y control de inventario en tiempo real.

# Sobre el proyecto

VentaRuta permite a los choferes registrar ventas, escanear productos y gestionar información directamente desde dispositivo móvil.

El sistema integra hardware como escáner Honeywell y utiliza base de datos local (SQLite) sincronizada con servicios externos.

# Enfoque QA

Durante el desarrollo se realizaron pruebas para asegurar el correcto funcionamiento del sistema en condiciones reales:

- Validación de escaneo de códigos con dispositivo físico  
- Pruebas funcionales en flujo de venta (escaneo → registro → pago)  
- Verificación de persistencia de datos en SQLite  
- Validación de sincronización con API  
- Pruebas en manejo de errores de conexión  

## Casos de prueba realizados

# Escaneo de productos
- Escaneo correcto de códigos válidos  
- Manejo de códigos inválidos o no registrados  
- Validación de lectura continua del escáner  

# Registro de venta
- Cálculo correcto de subtotal y total  
- Validación de productos agregados  
- Eliminación de productos sin afectar cálculo  

# Formas de pago
- Validación de selección obligatoria  
- Cálculo correcto de cambio en efectivo  
- Manejo de errores en datos incompletos  

# Sincronización
- Validación de envío de datos a servidor  
- Manejo de fallos de conexión  
- Prevención de duplicidad de registros  

# Ejemplos de errores detectados

- Fallos en sincronización de datos en conexión inestable  
- Errores en cálculo de totales en ciertos escenarios  
- Problemas en lectura continua del escáner  
- Inconsistencias en datos almacenados en SQLite  


# Tecnologías utilizadas

- Flutter  
- Dart  
- SQLite  
- APIs REST  
- Escáner Honeywell (EDA5)  
- Impresoras térmicas  


# Capturas

<img width="297" height="535" alt="image" src="https://github.com/user-attachments/assets/c1b9a47e-3385-4f9a-93cf-575346c7b708" />

---

<img width="373" height="641" alt="image" src="https://github.com/user-attachments/assets/d407bb45-b2df-4ea1-998c-8e3bfc18e0e9" />




# Aprendizajes

- Validación de aplicaciones en entornos reales (campo)  
- Integración de hardware con software móvil  
- Importancia de pruebas en condiciones fuera de laboratorio  
- Manejo de errores en sistemas offline/online  


# Estado del proyecto

Sistema desplegado en producción. Mantenimiento y evolución a cargo de la empresa.


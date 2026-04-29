## Atributos de Calidad del Sistema

Nuestra plataforma digital de turismo inteligente está diseñada para ofrecer experiencias de viaje colaborativas mediante tecnología cloud-native, conectando viajeros con intereses similares y proporcionando recomendaciones personalizadas. La arquitectura asegura operación continua, seguridad empresarial y escalabilidad para soportar el crecimiento del negocio.

---

### Disponibilidad y Continuidad del Servicio

* **Fuente:** Usuarios finales y equipo de operaciones.
* **Estímulo:** Fallo inesperado de un servidor de procesamiento.
* **Entorno:** Operación normal del servicio en entorno cloud.
* **Artefacto:** Sistema de balanceo de carga y servidores redundantes.
* **Respuesta:** Detección automática del fallo y redistribución del tráfico a servidores saludables.
* **Medidas:** Tiempo máximo de interrupción por servicio inferior a 5 minutos; disponibilidad del servicio superior al 99.5%; capacidad de atender hasta 3 instancias simultáneas por servicio.

---

### Escalabilidad para Crecimiento del Negocio

* **Fuente:** Aumento natural de usuarios y transacciones.
* **Estímulo:** Incremento sostenido de la demanda del servicio.
* **Entorno:** Operación comercial con picos de demanda estacional.
* **Artefacto:** Sistema de escalado automático de servidores.
* **Respuesta:** Adición automática de capacidad de procesamiento según la demanda.
* **Medidas:** Capacidad de escalar entre 1-3 servidores para el servicio principal y 1-2 para inteligencia artificial; utilización de CPU mantenida entre 20-70%; procesamiento de hasta 100 eventos pendientes en cola.

---

### Rendimiento en Condiciones de Alta Demanda

* **Fuente:** Usuarios interactuando con la plataforma.
* **Estímulo:** Picos de actividad simultánea en el sistema.
* **Entorno:** Operación con recursos optimizados para costos.
* **Artefacto:** Sistema de procesamiento y colas de trabajo asíncrono.
* **Respuesta:** Mantenimiento del servicio con degradación controlada del rendimiento.
* **Medidas:** Tiempo de respuesta percentil 95 inferior a 2 segundos; procesamiento de eventos sin pérdida de datos; ausencia de errores críticos sostenidos.

---

### Seguridad y Control de Acceso

* **Fuente:** Usuarios y clientes de la plataforma.
* **Estímulo:** Intentos de acceso no autorizado a funcionalidades protegidas.
* **Entorno:** Operación normal con autenticación requerida.
* **Artefacto:** Sistema de autenticación y control de permisos.
* **Respuesta:** Bloqueo inmediato de accesos no autorizados con registro del incidente.
* **Medidas:** Tasa de accesos bloqueados del 100% para credenciales inválidas; tiempo de sesión seguro configurado según política; cero operaciones no autorizadas persistidas.

---

### Seguridad de la Infraestructura

* **Fuente:** Tráfico externo desde Internet.
* **Estímulo:** Intentos de acceso directo a componentes internos.
* **Entorno:** Entorno de producción con red aislada.
* **Artefacto:** Sistema de protección de red y filtrado de tráfico.
* **Respuesta:** Bloqueo de accesos no autorizados y enrutamiento seguro del tráfico.
* **Medidas:** Cero accesos directos a bases de datos desde Internet; todo el tráfico encriptado; puertos de gestión restringidos según política.

---

### Seguridad en el Desarrollo y Despliegue

* **Fuente:** Equipo de desarrollo realizando cambios.
* **Estímulo:** Incorporación de código con vulnerabilidades o dependencias inseguras.
* **Entorno:** Proceso de desarrollo e integración continua.
* **Artefacto:** Sistema automatizado de análisis de seguridad.
* **Respuesta:** Bloqueo automático del despliegue si se detectan vulnerabilidades críticas.
* **Medidas:** Cero despliegues con vulnerabilidades críticas/altas; tiempo de detección de problemas inferior a 10 minutos; correlación de hallazgos con correcciones aplicadas.

---

### Monitoreo y Gestión Operativa

* **Fuente:** Equipo de operaciones y soporte técnico.
* **Estímulo:** Incidentes de rendimiento o errores del sistema.
* **Entorno:** Operación continua con supervisión activa.
* **Artefacto:** Sistema de monitoreo centralizado y alertas automáticas.
* **Respuesta:** Detección inmediata de anomalías y notificación al equipo responsable.
* **Medidas:** Tiempo de detección de incidentes inferior a 1 minuto; cobertura de monitoreo del 100% de servicios; tiempo medio de recuperación operativa documentado.

---

### Fiabilidad de Procesamiento Asíncrono

* **Fuente:** Sistema generando eventos de negocio.
* **Estímulo:** Volumen variable de eventos procesados en cola.
* **Entorno:** Operación con posibles demoras temporales.
* **Artefacto:** Sistema de mensajería garantizada.
* **Respuesta:** Retención y procesamiento garantizado de todos los eventos.
* **Medidas:** Profundidad de cola controlada bajo 100 eventos; retención de mensajes hasta 14 días; tasa de procesamiento exitoso superior al 99%.

---

### Mantenibilidad y Evolución del Sistema

* **Fuente:** Equipo de desarrollo implementando mejoras.
* **Estímulo:** Cambios funcionales o ajustes de negocio.
* **Entorno:** Desarrollo evolutivo con múltiples componentes.
* **Artefacto:** Arquitectura modular con componentes independientes.
* **Respuesta:** Implementación de cambios sin afectar todo el sistema.
* **Medidas:** Impacto del cambio limitado a componentes específicos; calidad de código mantenida según estándares; tiempo de compilación por componente optimizado.

---

### Compatibilidad e Integración

* **Fuente:** Aplicaciones cliente consumiendo servicios.
* **Estímulo:** Interacción entre diferentes componentes del sistema.
* **Entorno:** Operación con múltiples clientes y servicios.
* **Artefacto:** Interfaces estandarizadas y documentadas.
* **Respuesta:** Comunicación confiable entre componentes con intercambio de datos estructurado.
* **Medidas:** Tasa de errores de integración inferior al 1%; compatibilidad verificada con pruebas; versionado controlado de interfaces.

---

### Despliegue y Portabilidad

* **Fuente:** Equipo de plataforma gestionando infraestructura.
* **Estímulo:** Creación o recreación de entornos de operación.
* **Entorno:** Proceso de despliegue automatizado.
* **Artefacto:** Sistema de infraestructura como código.
* **Respuesta:** Creación reproducible de entornos completos de operación.
* **Medidas:** Tiempo de despliegue completo inferior a 2 horas; automatización del 95% de los pasos; consistencia garantizada entre entornos.

---

### Integridad y Recuperación de Datos

* **Fuente:** Operaciones de mantenimiento o incidentes.
* **Estímulo:** Pérdida de datos o necesidad de restauración.
* **Entorno:** Operación con copias de seguridad automáticas.
* **Artefacto:** Sistema de respaldo y recuperación gestionado.
* **Respuesta:** Restauración completa del estado anterior a un incidente.
* **Medidas:** Ventana de recuperación de 7 días; tiempo de restauración proporcional al volumen de datos; integridad verificada tras recuperación.

---

### Experiencia de Usuario Móvil

* **Fuente:** Viajeros utilizando la aplicación móvil.
* **Estímulo:** Condiciones variables de conectividad a red.
* **Entorno:** Operación móvil con conectividad limitada.
* **Artefacto:** Sistema de almacenamiento local y sincronización inteligente.
* **Respuesta:** Funcionalidad continua con datos recientes disponibles localmente.
* **Medidas:** Tiempo de carga de pantallas clave inferior a 1 segundo con datos locales; tasa de recuperación ante interrupciones superior al 95%; experiencia sin bloqueos de interfaz.

---

## Resumen de Garantías de Servicio

| Atributo de Negocio | Garantía Principal | Consideraciones Estratégicas |
|---------------------|-------------------|------------------------------|
| **Disponibilidad** | 99.5% de tiempo de actividad | Escalado limitado por recursos actuales |
| **Rendimiento** | Respuesta bajo 2 segundos (p95) | Optimizado para costos operativos |
| **Seguridad** | Bloqueo 100% de accesos no autorizados | Equilibrio entre seguridad y operatividad |
| **Escalabilidad** | Crecimiento automático hasta 3x capacidad | Preparado para expansión futura |
| **Recuperación** | Restauración completa en 7 días | Proceso manual requiere especialización |
| **Calidad** | Cero vulnerabilidades críticas en producción | Requiere proceso disciplinado de desarrollo |

Estos atributos aseguran que nuestra plataforma ofrezca un servicio confiable, seguro y escalable, soportando el crecimiento del negocio mientras mantienes la confianza de nuestros usuarios y stakeholders.

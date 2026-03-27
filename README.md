# KidCare_Repository
Sistema de bitácora de síntomas pediátricos para consulta médica con resumen asistido por IA
El proyecto consiste en el desarrollo de una plataforma digital compuesta por una aplicación móvil y una aplicación web que permitirá a los padres o tutores registrar y organizar las observaciones de síntomas que presentan sus hijos en días previos a una consulta médica, facilitando la comunicación con el profesional de salud durante la atención. La plataforma desea incluir un asistente de inteligencia artificial que organiza y resume las observaciones registradas y en una nueva actualización futura, un foro de padres
Actualmente los padres no cuentan con una herramienta estructurada para registrar las observaciones sobre los síntomas de sus hijos entre consultas médicas. Esta información suele olvidarse o comunicarse de forma imprecisa durante la atención, dificultando que el profesional de salud obtenga un relato completo del cuadro. Además, no existe un canal seguro para que los padres compartan estas observaciones previas con el médico tratante antes o durante la consulta. A esto se suma la falta de espacios digitales donde los padres puedan intercambiar experiencias sobre la crianza y el cuidado de la salud de sus hijos, lo que se considera una necesidad identificada que podría abordarse en una etapa futura del proyecto mediante la incorporación de un foro parental
Desarrollar una plataforma digital que permita a los padres o tutores registrar y organizar las observaciones de síntomas de sus hijos de forma estructurada y cronológica, y compartirlas de manera segura con el profesional de salud y compartirlas de manera segura con el profesional de salud mediante códigos QR de acceso temporal. El sistema incorporará la API de Claude (Anthropic), modelo Sonnet, para organizar y resumir automáticamente las observaciones registradas en la bitácora, facilitando su lectura durante la consulta médica, sin reemplazar el criterio clínico del profesional de salud
Desarrollar una plataforma digital que permita a los padres o tutores llevar una bitácora de síntomas de sus hijos y compartirla de forma segura con el profesional de salud, incorporando la API de Claude (Anthropic), modelo Sonnet, como herramienta de apoyo para organizar y resumir las observaciones registradas, facilitando su comprensión durante la consulta médica.



●   	Diseñar y desarrollar una aplicación móvil para dispositivos Android que permita a los padres o tutores registrar, editar y eliminar observaciones de síntomas del menor de forma estructurada y cronológica.
●   	Implementar una aplicación web que permita al profesional de salud visualizar la bitácora de síntomas compartida, accediendo de forma segura mediante códigos QR de acceso temporal.
●   	Integrar la API de Claude (Anthropic), modelo Sonnet, como módulo de apoyo que organiza y resume las observaciones registradas en la bitácora, entregando al profesional de salud un resumen estructurado previo a la consulta, sin emitir diagnósticos ni reemplazar el criterio clínico.
●   	Implementar un sistema de acceso temporal mediante códigos QR(numérico) que permita compartir la bitácora de síntomas de forma segura y exclusiva con el pediatra tratante, con expiración automática del acceso una vez cumplido el tiempo definido.
●   	Desarrollar un módulo de gestión de perfiles de menores que permita a los padres o tutores registrar y actualizar los datos básicos de identificación del menor, asociándose correctamente a la bitácora de síntomas correspondiente.
●   	Implementar un sistema de autenticación y gestión de usuarios que garantice el acceso seguro a la plataforma según el rol correspondiente, diferenciando entre padres/tutores y profesionales de salud.


El sistema permitirá a los padres o tutores registrarse como usuarios donde podrán registrar y organizar observaciones de síntomas del menor y compartirlas temporalmente con el profesional de salud mediante códigos QR(ver) de acceso temporal. El sistema incluirá una aplicación móvil para los padres, una aplicación web para el pediatra y un backend encargado de la gestión de datos. La API de Claude (Anthropic), modelo Sonnet, se utilizará únicamente para organizar y resumir las observaciones registradas en la bitácora, sin emitir diagnósticos ni reemplazar el criterio clínico del profesional de salud. El desarrollo de un foro parental queda fuera del alcance de esta versión y se considera como una línea de trabajo futuro.
Entregables
Aplicación móvil Android funcional para registro de observaciones de síntomas
Aplicación web para visualización de la bitácora por el pediatra mediante QR
Backend con API REST desplegado en ambiente cloud mediante un proveedor PaaS a definir durante el desarrollo.
Módulo de integración con API de Claude (Anthropic), modelo Sonnet
Documentación técnica del proyecto
Informe de pruebas funcionales
Supuestos
Los padres o tutores cuentan con un dispositivo Android con acceso a internet
El pediatra tratante cuenta con acceso a un navegador web durante la consulta
Se asume la disposición voluntaria del profesional de salud para acceder a la bitácora mediante el código QR durante la consulta.
El equipo cuenta con acceso a la API de Claude (Anthropic) durante todo el desarrollo
MongoDB Atlas estará disponible como servicio cloud para la base de datos.(DynamoDB AWS)
El sistema se desarrollará durante el semestre académico vigente, con un plazo máximo de 16 semanas a partir del inicio oficial del proyecto.
Restricciones
El sistema no almacenará ni procesará fichas clínicas oficiales ni documentos médicos institucionales
La IA no emitirá diagnósticos, prediagnósticos ni recomendaciones clínicas de ningún tipo; esta restricción se implementa mediante instrucciones explícitas en el system prompt de la API de Claude, limitando su rol estrictamente al resumen de texto.
El sistema operará bajo el marco de la Ley 19.628 de Protección de Datos Personales, requiriendo consentimiento explícito del padre o tutor mediante aceptación de términos y condiciones al momento del registro.
El acceso del pediatra a la bitácora expirará automáticamente tras un período máximo de 24 horas desde su generación.
El sistema estará disponible únicamente para dispositivos Android en su versión móvil
No se implementará el foro parental en esta versión del proyecto
Los datos ingresados son de exclusiva responsabilidad del padre o tutor que los registra.
La aplicación se limitará a comentarios y acotaciones de los padres bajo su responsabilidad y criterio, y esto no tendrá peso o intervención en ningún aspecto médico o algún aspecto legales.






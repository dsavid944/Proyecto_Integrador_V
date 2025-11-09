                                                    Evidencia de aprendizaje No. 1

                                                    Formulación de una necesidad de ingeniería de datos

                                                    Proyecto Integrado V

                                                    PREICA2502B020074

                                                    Eder David Sánchez Usuga


                                                    Andres Felipe Callejas


                                                    Noviembre 2025
 
 
Problema
Necesidad: priorizar puntos críticos de siniestralidad vial en Medellín para orientar intervenciones (señalización, operativos, campañas y educación).
Para quién: Secretaría de Movilidad, Planeación, Policía de Tránsito y equipos de seguridad vial.
Por qué requiere analítica: el fenómeno es multivariable y espaciotemporal; se necesita integrar y analizar fecha/hora, clase y gravedad del incidente, además de comuna/barrio y ubicación geográfica (X/Y) para detectar hotspots, comportamientos por franja horaria y tendencias interanuales que respalden decisiones basadas en datos.
 
Dataset elegido
•	Título: Incidentes viales
•	Fuente/Portal: MEData (Alcaldía de Medellín)
•	Editor/Publicador: Secretaría de Movilidad de Medellín
•	Identificador: 1-023-25-000094
•	Cobertura temporal: desde 2014-01-01T00:00:00Z
•	Frecuencia: Anual
•	Fecha de publicación: 28-12-2020
•	Última modificación: 01-02-2023
•	Catálogo (ficha): Incidentes viales (MEData). 
•	Descarga (CSV): distribución con ID 1-023-25-000094 (encabezados: AÑO, CBML, CLASE_ACCIDENTE, …, X, Y). 
•	Licencia: Creative Commons BY-SA 4.0 (legalcode). 
•	Estándar de datos: MinTIC (referenciado por el catálogo). 

Descripción oficial resumida: Incidentes de tránsito registrados por la Secretaría de Movilidad desde 2014 (definición de incidente según Ley 769 de 2002; IPAT como fuente operativa).
 
Variables relevantes
1.	FECHA_ACCIDENTES / FECHA_ACCIDENTE
Permite derivar fecha y hora del evento para analizar picos por franja horaria, días/temporadas y detectar patrones temporales.
2.	CLASE_ACCIDENTE
Identifica el tipo de suceso (p. ej., Choque, Atropello, Volcamiento). Útil para tipificar riesgos y orientar intervenciones específicas (infraestructura peatonal, pacificación de velocidad, etc.).
3.	GRAVEDAD_ACCIDENTE
Indica la severidad (Sólo daños, Herido, Muerto). Sirve para priorizar zonas no solo por frecuencia sino por impacto en la seguridad vial.
4.	COMUNA / NUMCOMUNA
Soporta la agregación territorial y la focalización de recursos por comunas; base para tableros y mapas comparativos entre territorios.
5.	BARRIO
Brinda mayor granularidad espacial para localizar micro-hotspots dentro de cada comuna y planear acciones puntuales.
6.	X y Y (MAGNA Medellín Local)
Coordenadas para análisis geoespacial (mapas de calor, clústeres). Se pueden reproyectar a WGS84 si se requieren visualizaciones web o en SIG.
7.	DISENO
Describe el sitio vial (Intersección, Glorieta, Tramo de vía, etc.). Ayuda a correlacionar la morfología de la vía con la ocurrencia y severidad de los incidentes. 
Referencias
Secretaría de Movilidad de Medellín (MEData). (28 de 12 de 2020). https://medata.gov.co. Obtenido de https://medata.gov.co/dataset/1-023-25-000094






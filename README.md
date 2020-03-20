# COVID-19 <!-- omit in toc -->

## Tabla de contenido <!-- omit in toc -->
- [Información del repositorio](#información-del-repositorio)
- [Investigadores que colaboran en el repositorio](#investigadores-que-colaboran-en-el-repositorio)
- [¿Por qué debemos quedarnos en casa?](#por-qué-debemos-quedarnos-en-casa)
- [Referencias](#referencias)
  - [Links a noticias](#links-a-noticias)
    - [Casos asintomáticos](#casos-asintomáticos)
    - [Noticias de medidas contra el COVID-19 en Colombia](#noticias-de-medidas-contra-el-covid-19-en-colombia)
    - [Modelación basada en agentes para entender el contagio](#modelación-basada-en-agentes-para-entender-el-contagio)
    - [Noticias y datos de casos en Colombia](#noticias-y-datos-de-casos-en-colombia)
    - [Links adicionales](#links-adicionales)
  - [Referencias a documentos científicos](#referencias-a-documentos-científicos)
    - [Genómica del COVID-19](#genómica-del-covid-19)
    - [Casos asintomáticos](#casos-asintomáticos-1)
  - [Material multimedia de interés](#material-multimedia-de-interés)
    - [Lucha contra el COVID-19](#lucha-contra-el-covid-19)
    - [Noticias de medidas contra el COVID-19 en Colombia](#noticias-de-medidas-contra-el-covid-19-en-colombia-1)
- [Conflicto de intereses](#conflicto-de-intereses)

# Información del repositorio

Este repositorio contiene varios códigos en Python que se hacen públicos con el
fin de ayudar en la investigación alrededor del COVID-19, y también de educar a 
las personas frente a las simulaciones epidemiológicas que deben conocer para 
tomar decisiones que ayuden a la prevención contra su contagio.

Intentaremos que este repositorio tenga simulaciones, links a
artículos de prensa y científicos, y contenido mutlimedia que sea relevante
para enfrentar esta pandemia. Nuestro propósito es informar respecto a la lucha 
contra el COVID-19.

Invitamos a otros investigadores a que se sumen a este esfuerzo uniéndose al
repositorio.


# Investigadores que colaboran en el repositorio

A continuación listamos los investigadores que han estado trabajando en estos
códigos:

- Boris Anghelo Rodriguez Rey
  - Profesor de Física, Universidad de Antioquia
  - [CvLAC](http://scienti.colciencias.gov.co:8081/cvlac/visualizador/generarCurriculoCv.do?cod_rh=0000057681), [Perfil en Google Scholar](https://scholar.google.com/citations?user=swUKsPkAAAAJ&hl=es)
- Isabel Cristina Hoyos Rincón
  - Profesora de Física, Universidad del Quindío
  - [CvLAC](https://scienti.minciencias.gov.co/cvlac/visualizador/generarCurriculoCv.do?cod_rh=0000236594), [Perfil en Google Scholar](https://scholar.google.com/citations?user=YzeNe7EAAAAJ&hl=es)
- Gloria Machado Rodriguez
  - Profesora de Biología, Universidad de Antioquia
  - [CvLAC](https://scienti.minciencias.gov.co/cvlac/visualizador/generarCurriculoCv.do?cod_rh=0000028061)
- Camilo Hincapié Gutiérrez
  - Científico de Datos, MSc en Física, Universidad de Antioquia
  - [CvLAC](https://scienti.minciencias.gov.co/cvlac/visualizador/generarCurriculoCv.do?cod_rh=0001494583), [Perfil en LinkedIn](https://www.linkedin.com/in/camilo-hincapie-gutierrez/)
- Nicole Rivera Parra
  - Estudiante de Física, Grupo de Fundamentos y Enseñanza de la Física y los 
    Sistemas dinámicos, Universidad de Antioquia

Debemos agradecer la colaboración de los siguientes colegas y estudiantes que a 
lo largo de esta semana han participado de las discusiones de estas ideas, han 
proveído de artículos, datos, códigos y análisis adicionales, y reflexiones.

- Jeison Rojas, Estudiante de Física, Universidad del Quindío.
- Yordi Sebastián Tamayo Molina, Estudiante de Biología, UdeA.
- Shirley Patricia Carcamo Londoño, Bióloga, UdeA.
- Valentina Ramírez Maldonado, Bióloga UdeA, Estudiante de Doctorado, 
  Universidad de Salamanca.
- Amalia Llano Bojanini, Bióloga UdeA, Estudiante de Maestría, Universidad de Amsterdam.
- Lina Marcela Ruiz Galvis, Bióloga UdeA, Estudiante de Maestría en Biología, UdeA.
- Juan Camilo Arboleda Rivera, Biólogo UdeA, Estudiante de Maestría en Biología, UdeA.
- Ghennie Tatiana Rodríguez Rey, Prof. de Biología, Universidad de Caldas.
- Jayson Gutierrez, Biólogo UdeA, Postdoc, Flanders Marine Institute, Bélgica.


# ¿Por qué debemos quedarnos en casa?

Con preocupación vemos que existe todavía mucha desinformación respecto a la 
pandemia que enfrentamos. Las medidas gubernamentales en Colombia resultan
insuficientes a la luz de los estudios de investigadores a nivel mundial y
parecen ignorar lo delicado del asunto, en cuanto a salud pública se refiere.

En especial encontramos preocupante que las estadísticas que se comparten con 
la comunidad solamente incluyen el número de individuos diagnosticados. En el 
país nos estamos olvidando que  existe un subregistro muy alto de este número 
([Substantial undocumented infection facilitates the rapid dissemination of novel coronavirus (SARS-CoV2)][asintomaticos 4]).
Se estima que en China hubo alrededor de un 86% de los infectados 
que presentaban síntomas muy leves --fácilmente confundibles con gripe común-- 
o inclusive **asintomáticos**, lo cual en sí mismo es aún más grave, ya que los 
estudios han mostrado que dichos individuos que no presentan síntomas sí pueden
contagiar el virus (ver [Infobae: Los “transmisores silenciosos” que propagan el coronavirus: las personas sin síntomas también contagian][asintomaticos 1], [redaccionmedica.com: Coronavirus sin síntomas: ¿se puede transmitir la enfermedad?][asintomaticos 2], [Substantial undocumented infection facilitates the rapid dissemination of novel coronavirus (SARS-CoV2)][asintomaticos 4]). Señalamos comentarios importantes al respecto:

> En términos prácticos, el estudio internacional plantea un problema urgente:
> si “la elevada proporción de casos no documentados", simplemente porque no 
> mostraron síntomas, "parece haber facilitado la rápida propagación del virus 
> en toda China”, entonces no se sostiene el criterio (sobre el que han 
> insistido algunas autoridades en el mundo) de no hacerle el examen a quienes 
> no presentan señales: podrían ser portadores sanos del coronavirus. 
> 
> Al contrario, los expertos subrayaron: “Se necesitaría un aumento radical de 
> la identificación y el aislamiento de las infecciones actualmente no 
> documentadas para controlar plenamente el SARS-CoV2”.
> > Fuente: [Infobae: Los “transmisores silenciosos” que propagan el coronavirus: las personas sin síntomas también contagian][asintomaticos 1]

El caso de China muestra que la cuarentena es altamente efectiva cuando la
situación comienza a salirse de control. Sin embargo, el caso de Corea del Sur,
y todas las medidas aplicadas por su gobierno --entre las cuales está realizar
**exámenes de diagnóstico masivo** a sus ciudadanos, presenten o no presenten
síntomas--, ayudó a un diagnóstico temprano e inclusive a detectar aquellos que
no presentaban síntomas, lo que llevó a que se pudieran tomar medidas de 
**aislamiento preventivo** y así contener la propagación. 
Vale mencionar que en el caso de Corea del Sur, la población se tomó en serio 
este virus y obedecieron las medidas de **auto-aislamiento**, lo cual 
finalmente ayudó a no tener la necesidad de obligar a todo el país a entrar en 
cuarentena.

En contraste con estos dos países, encontramos los casos de Italia y España, que
no tomaron las medidas de contención del virus a tiempo y ahora están en serias
dificultades. Hay un dato especial hoy, Italia está cambiando las estadísticas
al presentar 475 muertos en 24 horas, superando lo que se sabía del 
brote de China. Adicional, se debe tener en cuenta la tasa de mutación y 
adaptación del virus, que ya se puede ver con la dinámica de la evolución del 
virus ([Genomic epidemiology of novel coronavirus (hCoV-19)][covid-19 genomics]). 
Además, aunque se reporta a la fecha un 
índice de mortalidad de 0,2% a 0.4% para un rango de edades de 30-39 años y 
40-49 años de edad, respectivamente (infometers. COVID-19 Fatality Rate by AGE).
También, hay que tener en cuenta que estos datos corresponden a una selección 
sesgada, dado que cuando el sistema de salud colapsa y se tiene que decidir 
cuál vida salvar, se debe escoger la persona con mayor esperanza de vida.

Si no hay respiradores, no hay esperanza de vida que valga.

Un escenario preocupante para los colombianos y que está ligado con lo anterior 
es el hecho de que el primer caso de coronavirus reportado en China fué en 17 
de noviembre de 2019 y en nuestra gran Feria de Colombiatex, que se llevó a 
cabo del 21 al 23 de enero de 2020, participaron 22 países, entre ellos China, 
quien tuvo 4 empresas, Italia quien tuvo 22 empresas, España quien tuvo 16 
empresas y Estados Unidos con con 16 empresas entre otros, y Colombia con más 
de 300 empresas, 
([Colombiatex 2020 - Listado de expositores][colombiatex]) 
aunado al Fashion Week Madrid 2020 que se llevó a cabo del 28 de enero al 02 de 
febrero y el Milan Fashion Week que se llevó a cabo del 18 al 24 de febrero 
de 2020. Ferias en las cuales participan los empresarios de la moda de Colombia. 

¿Qué significa lo anterior? La cepa viral originaria de China es muy probable 
que llegara a suelo colombiano en enero y se dispersó entre los participantes 
de la Colombiatex y/o aeropuertos, aviones, lugares turísticos etc., 
posteriormente los empresarios colombianos que fueron a Madrid y Milán, al 
retornar al país en febrero, sin ninguna precaución ni cuarentena, retornaron 
con la cepa viral mejorada. No es de extrañar que nuestro pico sea mucho más 
alto puesto que el personal de las empresas de Brescia, Vicenza, Lombardía, 
Bérgamo y Milán, estuvieron presentes en el evento colombiano en enero y 
colombianos tanto empresarios de la moda como turistas estuvieron en Europa 
entre enero y febrero. Todo esto aunado al alto índice de turismo de los 
ciudadanos chinos en el mundo. A nivel de la comunidad europea, se reporta que 
son las personas que más gastan en turismo y para Medellín el índice de 
ocupación hotelera fue bastante alto en los meses de enero y febrero 
([Sistema de Indicadores Turísticos MEdellín-Antioquia: Porcentaje ocupación hotelera mensual por zona][situr]).

Se debe tener en cuenta que han aparecido reportajes y estudios en los cuales
se afirma que existen dos cepas del virus:

- La cepa inicial de China, que es la más leve y a la cual pertenecen los casos
  de contagio de ese país durante el mes de diciembre.
- La cepa modificada de febrero, la cual se ha esparcido por Milán, y se ha 
  catalogado como más agresiva que la anterior

Si a esto sumamos el hecho de encontrar reportajes en los cuales se afirma 
que "Según Migración Colombia y el Aeropuerto Rafael Núñez, solo en enero 
llegaron entre 7 y 20 italianos diarios a Cartagena" y que "llegaron el viernes
a Bogotá y se les hizo control migratorio y encuesta para ingresar y todos la 
pasaron, ninguno presenta síntomas" (ver [El Heraldo: “Los turistas italianos que están en Cartagena no tienen síntomas de coronavirus”][Colombia asintomaticos 1]). Lo cual parece indicar 
que los controles migratorios no han realizado las pruebas adecuadas para 
evitar el contagio por contacto con personas asintomáticas. De hecho, los
reportajes locales evidencian que algunos de los diagnosticados han incumplido
normas de **aislamiento preventivo** por no sentir síntomas (ver [El Tiempo: Joven con coronavirus violó cuarentena en Bogotá y voló a Cartagena][Colombia asintomaticos 2]).

Nuestro país, a fecha de hoy 19/Marzo/2020, cuenta con 128 casos confirmados de 
Coronavirus (ver [Coronavirus (COVID - 2019) en Colombia][Casos Colombia 1]), 
de los cuales 82 son importados de otros países --es decir que se 
contagiaron fuera del país y a su llegada a Colombia, y ya instalados en sus 
hogares comenzaron a presentar síntomas-- y los 44 restantes corresponden a 
casos asociados --es decir que se contagiaron por contacto con estos casos 
importados--. 

En un estudio realizado por los docentes Tatiana González Pérez y 
Luis Perdomo Hurtado, de la Universidad Autónoma de Manizales, se determinó que
Colombia es uno de los países con mayor número de casos confirmados en más poco 
tiempo (ver [Colombia, país con mayor número de casos covid-19 en menor tiempo][Casos Colombia 2]). 
Se resalta los siguientes comentarios importantes:

> Si bien en América latina, en ningún país los casos sobrepasan las 300 
> personas, el brote de los casos ha sido más rápido a comparación de los otros 
> países analizados.
>
> El ritmo en cada país es diferente. En España e Italia hasta el día 20 de la 
> aparición de la enfermedad había aumentado paulatinamente, pero a partir de 
> éste, se presentó un aumento repentino del brote. 
> 
> Colombia es el país que ha tenido más número de casos en más poco tiempo. 
> Es decir, al día 11 en Colombia (hoy) tenemos 57 casos confirmados, 
> al día 11 en otros países como Italia se tenían 3 casos, en Estados Unidos 8 
> casos, en Brasil 20 casos  y en Ecuador 17 casos confirmados.
> (Datos fuente de “Johns Hopkins Coronavirus Resource Center” y del 
> “Instituto Nacional de Salud de Colombia INS”).
>
> “Aunque el panorama se torna difícil, en Colombia tenemos la posibilidad de 
> tomar las medidas a tiempo, la experiencia que nos deja China es que la clave
>  para contener un brote es reducir el ritmo al que crecen los casos y esto 
> solo se consigue con el aislamiento social, por ejemplo, una cuarentena”, 
> dijeron los docentes de la UAM.
>
> Esta información debe ser usada como evidencia científica para tomar medidas 
> contundentes y hacer un llamado a las autoridades municipales y 
> departamentales para que aumenten las medidas de atenuación.
> 
> > Fuente: [Colombia, país con mayor número de casos covid-19 en menor tiempo][Casos Colombia 2]

Además de lo anterior, al hacer un ejercicio simple de porcentajes, si 
solamente el 14% de la población presenta síntomas, podemos entonces esperar 
que en total en el país existan:

> 128 casos equivalen al 14%  entonces tendríamos 914 casos totales

Es decir que si dicha estadística es correcta, entonces tendríamos 786 casos 
no diagnosticados, ya que no presentan síntomas pero sí pueden transmitir el
virus. Estamos en una situación que es un juego de estadística y probabilidades,
en la cual es mejor estar seguros que estar con incertidumbre. 
Como dice el dicho:

> El prudente se anticipa al peligro y toma precauciones.
> 
> El imprudente avanza a ciegas y sufre las consecuencias.

Hasta el momento, las medidas de Colombia han sido habilitar canales de 
reporte y diagnóstico para que aquellos que tengan síntomas se hagan el examen,
sin embargo, esto se traduce en que el contagiado asintomático nunca llame, por no
presentar síntomas, y en su lugar  siga transmitiendo el virus sin saberlo. 
Debemos entender que, hasta no tomar medidas como las tomadas por Corea del Sur 
de **diagnóstico masivo**, los casos no diagnosticados seguirán propagando el 
virus. Es necesario que se establezcan medidas más drásticas de diagnóstico y 
control para quienes llegan al país
y para quienes se transportan a través de él, de tal manera que por su
bienestar y el de todos, podamos controlar el brote de **COVID-19** en nuestro 
país. De hecho, el Gobierno Nacional ha llamado al orden respecto a las medidas
que deben tomarse y a centralizar las decisiones, sin embargo los noticieros 
locales reportan (ver [Noticias Caracol: Duque asume control total de decisiones para enfrentar el coronavirus en Colombia][medida 1], [El Universal: Gobierno y comercio piden a alcaldes no decretar toques de queda innecesarios][medida 2]) que hay preocupación en el ambiente porque los
gobernantes locales están intentando contener algo invisible y desconocido, ya 
que sin las medidas de **diagnóstico masivo** y posterior 
**aislamiento preventivo** seguiremos sin saber cómo se está propagando el 
virus realmente, y podríamos terminar con un escenario como el que se está 
viviendo en Europa. De hecho, en ese continente ya están adoptando las medidas
de prevención para diagnosticar a aquellos que son asintomáticos (ver [World Economic Forum: Could this be the way to eliminate COVID-19 faster?][Italia 1]).

Por otro lado, hay noticias positivas respecto a la forma 
en que algunas personas se están autorganizando para proveer a los vulnerables
y los necesitados (ver [Noticias Caracol: Moteros dan mercados a quienes sentirán el impacto económico por el aislamiento][voluntarios 1], [Voluntarios: Un Viejo Favor][voluntarios 2]). 

Concluimos diciendo, que adicional a las medidas que debe tomar el gobierno,
la población civil DEBE contribuir con el **auto-aislamiento preventivo** de la
misma manera que hicieron los ciudadanos de Corea del Sur. El Washington Post 
ha hecho una publicación de un [Corona-simulador][corona-simulator] donde a 
partir de una sencilla simulación explican la efectividad de esta medida.



# Referencias


## Links a noticias


### Casos asintomáticos

- [Infobae: Los “transmisores silenciosos” que propagan el coronavirus: las personas sin síntomas también contagian][asintomaticos 1]
- [redaccionmedica.com: Coronavirus sin síntomas: ¿se puede transmitir la enfermedad?][asintomaticos 2]
- [El Heraldo: “Los turistas italianos que están en Cartagena no tienen síntomas de coronavirus”][Colombia asintomaticos 1]
- [El Tiempo: Joven con coronavirus violó cuarentena en Bogotá y voló a Cartagena][Colombia asintomaticos 2]


[asintomaticos 1]: https://www.infobae.com/america/mundo/2020/03/18/los-transmisores-silenciosos-que-propagan-el-coronavirus-las-personas-sin-sintomas-tambien-contagian/
[asintomaticos 2]: https://www.redaccionmedica.com/secciones/sanidad-hoy/coronavirus-sintomas-asintomatico-transmitir-la-enfermedad--4552
[Colombia asintomaticos 1]: https://www.elheraldo.co/bolivar/los-turistas-italianos-que-estan-en-cartagena-no-tienen-sintomas-de-coronavirus-707590
[Colombia asintomaticos 2]: https://www.eltiempo.com/colombia/otras-ciudades/coronavirus-joven-que-habia-dado-positivo-en-bogota-viajo-a-cartagena-474076


### Noticias de medidas contra el COVID-19 en Colombia

- [Noticias Caracol: Duque asume control total de decisiones para enfrentar el coronavirus en Colombia][medida 1]
- [El Universal: Gobierno y comercio piden a alcaldes no decretar toques de queda innecesarios][medida 2]

[medida 1]: https://www.youtube.com/watch?v=0D09qce_Jsg
[medida 2]: https://www.eluniversal.com.co/colombia/gobierno-y-comercio-piden-a-alcaldes-no-decretar-toques-de-queda-innecesarios-YX2563247

### Modelación basada en agentes para entender el contagio

- [Washington Post: Why outbreaks like coronavirus spread exponentially, and how to "flatten the curve"][corona-simulator]

[corona-simulator]: https://www.washingtonpost.com/graphics/2020/world/corona-simulator/


### Noticias y datos de casos en Colombia

- [Coronavirus (COVID - 2019) en Colombia][Casos Colombia 1]
- [Colombia, país con mayor número de casos covid-19 en menor tiempo][Casos Colombia 2]

[Casos Colombia 1]: https://www.ins.gov.co/Noticias/Paginas/Coronavirus.aspx
[Casos Colombia 2]: https://www.autonoma.edu.co/noticias/colombia-pais-con-mayor-numero-de-casos-covid-19-en-menor-tiempo


### Links adicionales

- [Colombiatex 2020 - Listado de expositores][colombiatex]
- [Sistema de Indicadores Turísticos MEdellín-Antioquia: Porcentaje ocupación hotelera mensual por zona][situr]

[colombiatex]: https://colombiatex.inexmoda.org.co/es/listado-de-expositores/
[situr]: (https://situr.gov.co/estadisticas/DfMeOcuHotelZonaMensual/general)

___

## Referencias a documentos científicos


### Genómica del COVID-19

- [Genomic epidemiology of novel coronavirus (hCoV-19)][covid-19 genomics]

[covid-19 genomics]: https://nextstrain.org/ncov

### Casos asintomáticos

- [Informe Técnico Coronavirus - Ministerio de Sanidad Español - Fecha 17/Marzo/2020][asintomaticos 3]
- [Substantial undocumented infection facilitates the rapid dissemination of novel coronavirus (SARS-CoV2)][asintomaticos 4]

[asintomaticos 3]: Documentos/20200317%20-%20Informe%20Técnico%20Coronavirus%20-%20Ministerio%20de%20Sanidad%20Español.pdf
[asintomaticos 4]: Documentos/Substantial%20undocumented%20infection%20facilitates%20the%20rapid%20dissemination%20of%20novel%20coronavirus%20(SARS-CoV2).pdf


___

## Material multimedia de interés


### Lucha contra el COVID-19

- [World Economic Forum: Could this be the way to eliminate COVID-19 faster?][Italia 1]

[Italia 1]: https://www.linkedin.com/posts/world-economic-forum_covid19-coronavirus-activity-6646443506883670016-2ETM

### Noticias de medidas contra el COVID-19 en Colombia

- [Noticias Caracol: Moteros dan mercados a quienes sentirán el impacto económico por el aislamiento][voluntarios 1]
- [Voluntarios: Un Viejo Favor][voluntarios 2]
  
[voluntarios 1]: https://www.youtube.com/watch?v=AUl74OLPj4c
[voluntarios 2]: Imagenes/Voluntarios_Un_viejo_favor.jpeg

___

# Conflicto de intereses

Los colaboradores de este repositorio declara no tener conflictos de intereses.
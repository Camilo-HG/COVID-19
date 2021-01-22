# COVID-19 <!-- omit in toc -->

## Tabla de contenido <!-- omit in toc -->

- [Información del repositorio](#información-del-repositorio)
- [¿Por qué debemos quedarnos en casa?](#por-qué-debemos-quedarnos-en-casa)
- [Simulaciones](#simulaciones)
- [Investigadores que colaboran en el repositorio](#investigadores-que-colaboran-en-el-repositorio)
- [Referencias](#referencias)
  - [Documentos principales](#documentos-principales)
  - [Links a noticias](#links-a-noticias)
    - [Modelación basada en agentes para entender el contagio](#modelación-basada-en-agentes-para-entender-el-contagio)
    - [El peligro de los casos asintomáticos y noticias al respecto](#el-peligro-de-los-casos-asintomáticos-y-noticias-al-respecto)
    - [Datos de casos diagnosticados en Colombia](#datos-de-casos-diagnosticados-en-colombia)
    - [Noticias respecto a las medidas contra el contagio del COVID-19 en Colombia](#noticias-respecto-a-las-medidas-contra-el-contagio-del-covid-19-en-colombia)
    - [Links adicionales](#links-adicionales)
  - [Referencias a documentos científicos](#referencias-a-documentos-científicos)
    - [Modelo matemático de propagación del COVID-19](#modelo-matemático-de-propagación-del-covid-19)
    - [Genómica del COVID-19](#genómica-del-covid-19)
    - [Casos asintomáticos](#casos-asintomáticos)
    - [Informe técnico de España](#informe-técnico-de-españa)
  - [Material multimedia de interés](#material-multimedia-de-interés)
  - [Lucha contra el COVID-19](#lucha-contra-el-covid-19)
    - [Noticias positivas de medidas contra el COVID-19 en algunos sectores de Colombia](#noticias-positivas-de-medidas-contra-el-covid-19-en-algunos-sectores-de-colombia)
- [Conflicto de intereses](#conflicto-de-intereses)

## Información del repositorio

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

## ¿Por qué debemos quedarnos en casa?

Invitamos a leer el documento: [¿Por qué debemos quedarnos en casa?](Por_que_debemos_quedarnos_en_casa.pdf)

- English version: [¿Why do we need to stay home?](Why_do_we_need_to_stay_home.pdf)

Al final del mismo hacemos la siguiente reflexión:

> "A través de este documento queremos invitar a cada uno de los colombianos a
> adoptar medidas de auto-aislamiento preventivo. La información que hemos
> recopilado y los modelos que hemos diseñado pretenden proporcionar
> información significativa en la construcción de una opinión informada que nos
> permita, a cada uno de nosotros como habitantes de este planeta, tomar las
> decisiones que están en nuestras manos para enfrentar esta pandemia de una
> manera consciente y solidaria. Hoy tenemos la oportunidad de reconocer la
> fragilidad de la especie humana y de volver a valorar la vida en la medida
> que lo merece. El acto más generoso que podemos hacer hoy es el cuidado
> mutuo, entendiendo el enorme poder que tienen los pequeños esfuerzos
> cuando estos se suman, de la misma manera que lo hicieron los ciudadanos
> de Corea del Sur".

Estamos en una situación en la cual controlar la estadística y las
probabilidades es demasiado importante, pues es mejor estar seguros
que tener incertidumbre. Invitamos a que sea cual sea la situación en su propio
país, se tomen precauciones inmediatas:

> El prudente se anticipa al peligro y toma precauciones.
> El imprudente avanza a ciegas y sufre las consecuencias.

También hemos realizado el pronósticos para los siguientes países:

- [Propagación virus COVID-19 en Ecuador - Fecha: 23/Marzo/2020](Propagacion_Virus_Ecuador_23-Marzo-2020.pdf)
- [Propagación virus COVID-19 en Costa Rica - Fecha: 31/Marzo/2020](Propagacion_Virus_CostaRica_31-Marzo-2020.pdf)

También invitamos a leer el documento (más técnico): [Coronavirus: Colombia, a tres semanas de Italia. Todavía hay tiempo de actuar!! - 18/Marzo/2020](Documentos/ISPM_Coronavirus_en_Colombia.pdf)

## Simulaciones

- [Modelo epidemiológico de propagación del COVID-19](Simulaciones/Propagaci%C3%B3n_COVID-19_Colombia.ipynb)
- [Modelo Basado en Agentes (ABM) para la propagación del COVID-19](Simulaciones/ABM_COV-19_v0.5_DM.ipynb)

## Investigadores que colaboran en el repositorio

Esta iniciativa se originó en el **Grupo de Fundamentos y Enseñanza de la Física y los Sistemas Dinámicos**, específicamente por parte de los investigadores de la
línea de estudio de **Sistemas Complejos** y **Modelación de Sistemas**. A continuación
listamos los investigadores que han estado trabajando en estos
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
- Jayson Gutierrez, Biólogo UdeA, Postdoc, VLIZ Flanders Marine Institute, Bélgica.

## Referencias

### Documentos principales

- [¿Por qué debemos quedarnos en casa?](Por_que_debemos_quedarnos_en_casa.pdf)
- [¿Why do we need to stay home?](Why_do_we_need_to_stay_home.pdf)
- [Propagación virus COVID-19 en Ecuador - Fecha: 23/Marzo/2020](Propagacion_Virus_Ecuador_23-Marzo-2020.pdf)
- [Propagación virus COVID-19 en Costa Rica - Fecha: 31/Marzo/2020](Propagacion_Virus_CostaRica_31-Marzo-2020.pdf)
- [¿Por qué debemos seguir cuidándonos? - Fecha: 20/Enero/2021](Por_que_debemos_seguir_cuidandonosV2.pdf)

### Links a noticias

#### Modelación basada en agentes para entender el contagio

- [Washington Post: Why outbreaks like coronavirus spread exponentially, and how to "flatten the curve"](https://www.washingtonpost.com/graphics/2020/world/corona-simulator/)
- [Por qué brotes como el del coronavirus crecen exponencialmente y cómo "aplanar la curva"](https://www.washingtonpost.com/graphics/2020/world/corona-simulator-spanish/)

#### El peligro de los casos asintomáticos y noticias al respecto

- [Infobae: Los “transmisores silenciosos” que propagan el coronavirus: las personas sin síntomas también contagian](https://www.infobae.com/america/mundo/2020/03/18/los-transmisores-silenciosos-que-propagan-el-coronavirus-las-personas-sin-sintomas-tambien-contagian/)
- [redaccionmedica.com: Coronavirus sin síntomas: ¿se puede transmitir la enfermedad?](https://www.redaccionmedica.com/secciones/sanidad-hoy/coronavirus-sintomas-asintomatico-transmitir-la-enfermedad--4552)
- [El Heraldo: “Los turistas italianos que están en Cartagena no tienen síntomas de coronavirus”](https://www.elheraldo.co/bolivar/los-turistas-italianos-que-estan-en-cartagena-no-tienen-sintomas-de-coronavirus-707590)
- [El Tiempo: Joven con coronavirus violó cuarentena en Bogotá y voló a Cartagena](https://www.eltiempo.com/colombia/otras-ciudades/coronavirus-joven-que-habia-dado-positivo-en-bogota-viajo-a-cartagena-474076)

#### Datos de casos diagnosticados en Colombia

- [Coronavirus (COVID - 2019) en Colombia](https://www.ins.gov.co/Noticias/Paginas/Coronavirus.aspx)
- [Colombia, país con mayor número de casos covid-19 en menor tiempo](https://www.autonoma.edu.co/noticias/colombia-pais-con-mayor-numero-de-casos-covid-19-en-menor-tiempo)

#### Noticias respecto a las medidas contra el contagio del COVID-19 en Colombia

- [Noticias Caracol: Duque asume control total de decisiones para enfrentar el coronavirus en Colombia](https://www.youtube.com/watch?v=0D09qce_Jsg)
- [El Universal: Gobierno y comercio piden a alcaldes no decretar toques de queda innecesarios](https://www.eluniversal.com.co/colombia/gobierno-y-comercio-piden-a-alcaldes-no-decretar-toques-de-queda-innecesarios-YX2563247)

#### Links adicionales

- [Colombiatex 2020 - Listado de expositores](https://colombiatex.inexmoda.org.co/es/listado-de-expositores/)
- [Sistema de Indicadores Turísticos MEdellín-Antioquia: Porcentaje ocupación hotelera mensual por zona](https://situr.gov.co/estadisticas/DfMeOcuHotelZonaMensual/general)

___

### Referencias a documentos científicos

#### Modelo matemático de propagación del COVID-19

- [Yang, C. and Wnag, J., A mathematical model for the novel coronavirus epidemic in Wuhan, China (2020)](http://www.aimspress.com/article/10.3934/mbe.2020148)

#### Genómica del COVID-19

- [Genomic epidemiology of novel coronavirus (hCoV-19)](https://nextstrain.org/ncov)

#### Casos asintomáticos

- [Substantial undocumented infection facilitates the rapid dissemination of novel coronavirus (SARS-CoV2)](Documentos/Substantial%20undocumented%20infection%20facilitates%20the%20rapid%20dissemination%20of%20novel%20coronavirus%20(SARS-CoV2).pdf)

#### Informe técnico de España

- [Informe Técnico Coronavirus - Ministerio de Sanidad Español - Fecha 17/Marzo/2020](Documentos/20200317%20-%20Informe%20Técnico%20Coronavirus%20-%20Ministerio%20de%20Sanidad%20Español.pdf)

___

### Material multimedia de interés

### Lucha contra el COVID-19

- [VisualPolitik: ¿Cómo CHINA se ENFRENTÓ al CORONAVIRUS?](https://www.youtube.com/watch?v=PWTLSp7WOJY)
- [VisualPolitik: COREA: ¿Cómo GANAR al CORONAVIRUS sin BLOQUEAR un PAÍS?](https://www.youtube.com/watch?v=4ESWLnxyZUo)
- [World Economic Forum: Could this be the way to eliminate COVID-19 faster?](https://www.linkedin.com/posts/world-economic-forum_covid19-coronavirus-activity-6646443506883670016-2ETM)

#### Noticias positivas de medidas contra el COVID-19 en algunos sectores de Colombia

- [Noticias Caracol: Moteros dan mercados a quienes sentirán el impacto económico por el aislamiento](https://www.youtube.com/watch?v=AUl74OLPj4c)
- [Voluntarios: Un Viejo Favor](Imagenes/Voluntarios_Un_viejo_favor.jpeg)

___

## Conflicto de intereses

Los colaboradores de este repositorio declara no tener conflictos de intereses.

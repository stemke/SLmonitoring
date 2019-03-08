---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Métricas recopiladas (Beta)
Este tema cubre las métricas recopiladas para esta aplicación de supervisión beta en servidores virtuales y nativos.
{:shortdesc}

Este tema cubre todas las métricas disponibles mediante consultas de Grafana. Para obtener más información, consulte [Creación de una consulta de supervisión avanzada (Beta)](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-an-advanced-monitoring-query-beta-#creating-an-advanced-monitoring-query-beta-). Los gráficos están disponibles en la interfaz de usuario solo para las métricas siguientes:
* Utilización de CPU
* Uso de memoria
* Lectura y escritura de disco (bytes/segundos y E/S por segundo)
* Latencia de lectura y escritura de disco
* Rendimiento de red pública (entrada/salida)
* Rendimiento de red privada (entrada/salida)
* Paquetes de red pública (entrada/salida) (solo servidores nativos)
* Paquetes de red privada (entrada/salida) (solo servidores nativos)
* Errores de red pública (entrada/salida) (solo servidores nativos)
* Errores de red privada (entrada/salida) (solo servidores nativos)
* Temperatura (solo servidores nativos)


## Métricas de CPU
  Las métricas de CPU miden el porcentaje medio de tiempo que una CPU está ejecutando instrucciones durante un periodo de tiempo determinado. El porcentaje medio de desocupación es la desocupación debido a adición de usuario, sistema, espera de E/S, interrupciones de hardware e interrupciones de software.

## Medidas de memoria
* Bytes utilizados/Promedio utilizado: la cantidad de memoria que se utiliza en un momento dado, disponible tanto en bytes como en porcentaje del total.
* Bytes de intercambio utilizados/Promedio utilizado: el porcentaje de memoria de intercambio que se utiliza durante un determinado periodo de tiempo. Esta métrica es una indicación de la frecuencia con la que se deben recuperar los datos que no están en la memoria. Esta métrica solo está disponible en dispositivos nativos.

## Medidas de disco

* Total de disco: el número total de bytes disponibles para el disco. Esta métrica debe ser constante.
* Disco utilizado (bytes): el número de bytes que utiliza el disco en un determinado momento.
* Disco utilizado (porcentaje): el porcentaje del número total de bytes utilizados sobre el número total de bytes disponibles para el disco.
* Lectura/escritura de disco (bytes por segundo): la cantidad media de datos que se están leyendo/escribiendo desde/en disco en bytes durante un periodo de tiempo determinado.
* Lectura/escritura de disco (operaciones por segundo): operaciones de lectura/escritura por segundo
* Lectura/escritura de disco (latencia en ms por operación): latencia en ms por lectura/escritura

## Métrica de red

 * Entrada de red pública/privada: número de bytes enviados por la red pública/privada
* Salida de red pública/privada: número de bytes recibidos por la red pública/privada
* Entrada de paquetes de red pública/privada: número de paquetes recibidos por la interfaz de red en la red pública/privada. Esta métrica solo está disponible en dispositivos nativos.
* Salida de paquetes de red pública/privada: número de paquetes enviados por la interfaz de red en la red pública/privada. Esta métrica solo está disponible en dispositivos nativos.

## Medidas de temperatura
* Temperatura media del sistema medida en grados Celsius. Esta métrica solo está disponible en determinados dispositivos nativos.

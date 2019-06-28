 
# Librerias para **Codesys v2.3** y **eCockpit** 
## Símbolos
- :orange_book: Disponible para **Codesys v2.3** 
- :green_book:  Disponible para **eCockpit**
- :warning:  Hay diferencias funcionales entre la version para **Codesys v2.3** y **eCockpit**  
- :exclamation:  Hay diferencias en la interfaz entre la version para **Codesys v2.3** y **eCockpit**  


### WAGOIO :orange_book: :green_book:
Bloques de función para simplificar el trabajo con módulos de I/O
- **AI_FLEX**
Módulos de Entradas Analógicas 
- **AO_FLEX**
Módulos de Entradas Analógicas 

### WagoModusCoupler :orange_book: :green_book: 
Comunicacion con acopladores Modbus/Tcp.
- **WagoModbTcpCoupler** :green_book::warning: Comunicacion con acopladores Modbus/Tcp de WAGO (750-352 y similares). Tiene la opción del que el acoplador ponga todas sus salidas a cero, tanto analogicas como digitales, en el caso de que se interrumpan las comunicaciones.     

### DicoWagoSql :orange_book: :green_book:
Funciones auxiliares para las librerias de accesoa a Bases de Datos SQL de WAGO 
- **DTToRelianceTimeStamp** Convierte en variable de Fecha y Hora de tipo **DT** en el formato utilizado por **Reliance** en sus bases de datos. Se utiliza en aplicaciones donde el PLC escribe directamente en las tablas de la base de datos SQL.
- **DTToSqlDATETIME** Convierte en variable de Fecha y Hora de tipo **DT** en el formato del tipo **DATTETIME**  de las bases de  **SQL**, variable de tipo.
- **SqlCmdBuilder** :exclamation: Los comandos **SQL** se componen utilzando la estructura de datos __asSqlQuery__. Este bloque permite hacerlo de SQL de manera segura.

### DicoCollections :orange_book: :green_book:
Colecciones de datos    
- **RingFIFO** :exclamation: Gestion buffer circular con multiples consumidores. Este tipo de estructuras de detos son ideales en situaciones en los que la velocidad de procesado pueda ser lenta que las producción de los mismos, por ejemplo envío de alarmas mediente SMS.
- **RingFIFOFile** :exclamation: Igual que el anterior pero la informacion se almacena en un archivo en lugar de hacerlo en memoria. Se utiliza cuando se require que los datos sean persistentes y el PLC no tiene memoria retentiva suficiente. Al estar usar sistemas de almacenamiento flash y tener carater circular, es conveniente sobrediemensionar el tamaño del buffer para reducir el numero de escrituras sobre la misma celda de almancenamiento.       


### DicoStrUtil :orange_book: :green_book:
Funciones adicionales para manipular variables el tipo **__STRING__**  (texto)   


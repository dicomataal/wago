 
# Librerias para **Codesys v2.3** y **eCockpit** 
- :orange_book: Disponible para **Codesys v2.3** 
- :green_book:  Disponible para **eCockpit**

## WAGOIO :orange_book: :green_book:
Bloques de función para simplificar el trabajo con módulos de I/O
- **AI_FLEX**
Módulos de Entradas Analógicas 
- **AO_FLEX**
Módulos de Entradas Analógicas 

## WagoModusCoupler :orange_book: :green_book:
Comunicacion con acopladores Modbus/Tcp.
- **WagoModbTcpCoupler** Comunicacion con acopladores Modbus/Tcp de WAGO (750-352 y similares). Tiene la opción del que el acoplador ponga todas sus salidas a cero, tanto analogicas como digitales, en el caso de que se interrumpan las comunicaciones.     

- **DTToRelianceTimeStamp** Convierte en variable de Fecha y Hora de tipo **DT** en el formato utilizado por **Reliance** en sus bases de datos. Se utiliza en aplicaciones donde el PLC escribe directamente en las tablas de la base de datos SQL.

## DicoWagoSql :orange_book: :green_book:
Funciones auxiliares para las librerias de accesoa a Bases de Datos SQL de WAGO 
- **DTToRelianceTimeStamp** Convierte en variable de Fecha y Hora de tipo **DT** en el formato utilizado por **Reliance** en sus bases de datos. Se utiliza en aplicaciones donde el PLC escribe directamente en las tablas de la base de datos SQL.
- **DTToSqlDATETIME** Convierte en variable de Fecha y Hora de tipo **DT** en el formato del tipo **DATTETIME**  de las bases de  **SQL**, variable de tipo.
- **SqlCmdBuilder** Los comandos **SQL** se componen utilzando la estructura de datos __asSqlQuery__. Este bloque permite 
   hacerlo de SQL de manera segura.

## DicoStrUtil :orange_book: :green_book:
Funciones adicionales para manupilar variables el tipo **__STRING__**  (texto)   

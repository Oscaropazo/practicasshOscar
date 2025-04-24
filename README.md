# Tarea de SSH y SCP

## 1. Configuración de las máquinas virtuales

- Crear dos máquinas virtuales (A y B) con sus respectivos adaptadores de red:
  - Adaptador 1: tipo **NAT**
    - Una máquina con el reenvío de puertos predeterminado
    - La otra con el puerto **2223**
  - Adaptador 2: tipo **Red Interna**
    - Para permitir la comunicación entre ambas máquinas

![Paso 1](imagenes/imagen_1_1.png)

## 2. Conexión por SSH

- Conectarse por SSH a ambas máquinas
- Añadir los usuarios **Alex** y **Brais** en sus respectivas máquinas
- Configurar la IP en ambas máquinas

![Paso 2](imagenes/imagen_2_1.png)

## 3. Prueba de conexión

- Conectarse desde la máquina A a la máquina B
- Conectarse desde cada máquina a la otra y:
  - Crear un directorio en `/tmp`
  - Dejar un archivo como prueba de haberlo conseguido

![Paso 3](imagenes/imagen_3_1.png)

## 4. Copia de archivos

- Copiar desde cada máquina el archivo creado anteriormente
- Copiar esos archivos a la máquina nativa

![Paso 4](imagenes/imagen_4_1.png)

## 5. Prueba de carga masiva

- Crear el directorio `prueba3`
- Generar 200 archivos dentro del mismo
- Transferir ese directorio completo a la máquina nativa

![Paso 5](imagenes/imagen_5_1.png)

## 6. Autenticación con clave SSH

- Generar clave SSH en la máquina A
- Transferir la clave pública a la máquina B
- Verificar la conexión mediante autenticación por frase (clave)

![Paso 6](imagenes/imagen_6_1.png)

# Practica de SSH y SCP

## 1. Configuración de maquinas virtuales

- Crear dos máquinas virtuales A y B
  - Adaptador 1: tipo **NAT**
    - Una máquina con el puerto **2222**
    - La otra con el puerto **2223**
  - Adaptador 2: tipo **Red Interna**
    - Para la comunicación entre máquinas

![imagen](imagenes/imagen_1_1.png)

![imagen](imagenes/imagen_1_2.png)

## 2. Conexión por SSH

- Conectarse por SSH a las dos máquinas
- 
  ![imagen](imagenes/imagen_2_1.png)
  
![imagen](imagenes/imagen_2_2.png)

- Añadir los usuarios **Alex**, En la maquina A y **Brais** en la maquina B
  
  ![imagen](imagenes/imagen_2_3.png)
  
![imagen](imagenes/imagen_3_1.png)

- Configurar la IP de las máquinas

![imagen](imagenes/imagen_3_2.png)

![imagen](imagenes/imagen_3_3.png)

## 3. Prueba de conexión

- Conectar la máquina A a la máquina B

  ![imagen](imagenes/imagen_3_4.png)
  
- Conectar la maquina B a la maquiba A
  
    ![imagen](imagenes/imagen_4_1.png)
  
  - Crear un directorio en `/tmp`
  - Dejar un archivo como prueba

  ![imagen](imagenes/imagen_4_2.png)

## 4. Copia de archivos

- Copiar desde cada máquina el archivo que creamos antes
- Copiar esos archivos a la maquina real

![imagen](imagenes/imagen_4_3.png)

  ![imagen](imagenes/imagen_5_1.png)
  
## 5. Prueba de carga masiva

- Crear el directorio `prueba3`
- Generar denrto 200 archivos dentro del mismo
  
    ![imagen](imagenes/imagen_5_2.png)
  
- Transferir ese directorio completo a la máquina real

![imagen](imagenes/imagen_6_1.png)

## 6. Autenticación con clave SSH

- Generar clave SSH en la máquina A
  
    ![imagen](imagenes/imagen_6_2.png)
  
- Transferir la clave pública a la máquina B
  
    ![imagen](imagenes/imagen_7_1.png)

- Verificar la conexión mediante autenticación por frase
  
    ![imagen](imagenes/imagen_7_2.png)



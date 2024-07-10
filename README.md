#### 1. Iniciamos la maquina con el siguiente comando

[![start.png](https://i.postimg.cc/PxktV8Rv/start.png)](https://postimg.cc/06cRbrx9)

#### 2. Despues hacemos un ping para revisar si tenemos conectividad 

[![Virtual-Box-Debian-09-07-2024-22-58-45.png](https://i.postimg.cc/3rgrP9XS/Virtual-Box-Debian-09-07-2024-22-58-45.png)](https://postimg.cc/G9m1DFSG)

#### 3. Usamos "NMAP" para escanear los puertos de la maquina

[![nmap.png](https://i.postimg.cc/rmPbcnZx/nmap.png)](https://postimg.cc/njqTGkJh)

#### encontramos dos puertos 80 y 22 http y ssh

#### 4. Usamos Gobuster 

[![gob.png](https://i.postimg.cc/QtFDpWRg/gob.png)](https://postimg.cc/vgwCyD8D)

#### al usar gobuster nos encontramos "secret.php" al entrar nos encontramos esto:

[![web.png](https://i.postimg.cc/T2NVyrNc/web.png)](https://postimg.cc/DmsJHbTW)

####encontramos el usuario "mario" recuerdas que teniamos un puerto ssh pues ahora

#### 5. Usamos hydra para hacer un ataque

[![hy.png](https://i.postimg.cc/L6CvtcyG/hy.png)](https://postimg.cc/LnPzRbFV)

####vemos que nos da la contraseña de "chocolate" ahora que tenemos usuario y conraseña vamos a probarlo

[![ssh.png](https://i.postimg.cc/4dsFLzp0/ssh.png)](https://postimg.cc/GBgQ9T7P)

####vemos que funciono ahora tenemos que escalar privilegios

#### 6. Escalar privilegios

[![root.png](https://i.postimg.cc/Hx3cXgpN/root.png)](https://postimg.cc/R66Zx2J1)

#### ahora somos root

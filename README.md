# dockerizado-Nginx
---
****
1. Primero entramos en la web Docker hub y filtramos por nginx:

- ![image](https://user-images.githubusercontent.com/72273897/172397085-3b3b2ab1-12f4-435e-9422-e1de764f7f5f.png).

2. Hacemos el pull con sudo docker pull nginx 

3. Elevamos el contenedor que contiene el servicio nginx ejecutando el siguiente comando:
 docker run --rm -d -p 8080:80 --name web nginx.
 
4. Vemos que si entramos al localhots:8080, podremos visualizar la página default de nginx.
- ![Captura desde 2022-06-07 15-52-21](https://user-images.githubusercontent.com/72273897/172397675-82c455ab-2349-47e2-8f90-8b536b5ae23f.png).
5. A continuación, finalizamos el contenedor sudo docker stop web.
- ![Captura desde 2022-06-07 15-56-38](https://user-images.githubusercontent.com/72273897/172398746-27aa7d66-07bf-4581-857d-630b83411b66.png).

6. Procedemos a crear el index.html que emplearemos en nuestro nginx.
- ![Captura desde 2022-06-07 15-58-37](https://user-images.githubusercontent.com/72273897/172399273-34106a0a-6666-4e64-b682-41d55cb891cb.png).
- ![image](https://user-images.githubusercontent.com/72273897/172399674-c146766a-102c-4dfe-9ae0-2e1931501682.png).

7. Como vemos, al acceder ahora a nuestro hostlocal:8080, nos encontraremos con el index.html editado previamente.
- ![Captura desde 2022-06-07 16-04-20](https://user-images.githubusercontent.com/72273897/172400551-a35363b0-b53e-4c5e-bac2-e27cbb93ad47.png).

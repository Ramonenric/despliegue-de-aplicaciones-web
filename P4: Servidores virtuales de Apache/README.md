P4: Servidores virtuales de Apache

1. Crea dos sitios web que compartirán IP y puerto, pero tendrán nombres DNS distintos
para acceder a ellos. El nombre del primer dominio será daw.gimbernat.eug.es y el
segundo tunombreyapellidos.gimbernat.eug.es, donde “tunombreyapellidos” contiene
la inicial de tu nombre, el primer apellido, y la inicial de tu segundo apellido. De esta
manera, si tu nombre es: Francisco Mesas Cervilla, el domino quedaría:
fmesasc.gimbernat.eug.es.
• En el primer caso, daw.gimbernat.eug.es tendrá su directorio base en
/var/www/daw/ conteniendo una página llamada index.html que ponga el
nombre de la clase como título con un archivo css para aplicarle estilos al título.
• En el segundo caso, fmesasc.gimbernat.eug.es tendrá su directorio base en
/var/www/fmesasc/ (el equivalente para vuestros nombres), conteniendo una
página llamada index.html que contenga vuestro currículum aplicándole un
estilo css para que se visualice correctamente.
Para ello, tendrás que crear un archivo de configuración (copiado de 000-default.conf)
para cada uno de los dominios. Recuerda que con a2ensite puedes crear los enlaces
simbólicos necesarios para añadir esta configuración a la ejecución de apache.

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/92bf191d-f421-4f84-aff7-68e621d72959)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/261c1f4a-87d9-4416-80bc-8e5955d5c761)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/5bbc62a9-2a22-4299-a307-c2751ea009c5)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/323550b9-d46e-44fb-9d64-d8b8086ee6f9)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/9282916c-d0a4-420a-b5c0-ad3e41674274)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/554a37a9-318b-451c-8205-8c544b12b0d1)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/59bfe6f0-b37f-4f84-aa84-96a0895048b1)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/2c9259c3-26fd-4588-b55c-bc9126714c53)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/552b70f4-27de-4531-829a-438949b7290a)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/e15bd7cd-61f2-4a49-adbb-8a79baaf8aaf)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/5f73bc97-6c7f-42ba-a5ed-2452326792d7)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/2ed248ea-03ba-45e0-8995-21fc0a0796f6)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/2b33d789-3042-4b59-9f31-bacc68c8ebb6)

![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/16ba21f6-e79e-4483-b3d1-a684c5e31c4c)


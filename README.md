# Ejecutar proyecto de Alexa - Django - FastAPI
1. Tener una instancia con Docker, Git y Python instalado.
2. Clonar este repositorio.
3. Ingresar los valores de las variables de entorno en el archivo docker-compose.yml
- Base de datos: DB_HOST, DB_PORT, DB_DATABASE, DB_USERNAME, DB_PASSWORD
- API externa: EXTERNAL_API_HOST, EXTERNAL_API_PORT
- AWS: AWS_ACCESS_KEY_ID, AWS_DEFAULT_REGION, AWS_SECRET_ACCESS_KEY
- OpenAI: OPENAI_API_KEY
- Pinecone: PINECONE_API_KEY
- S3 Bucket: BUCKET_NAME # Nombre del bucket de S3 tener en cuenta que el bucket debe estar creado previamente
4. Ejecutar el comando `docker-compose up` en la raíz del proyecto.
5. Ingresar a la URL de la instancia en el puerto 80 para acceder a la aplicación de Django y en el puerto 8000 para acceder a la aplicación de FastAPI.
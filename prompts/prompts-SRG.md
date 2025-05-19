# Prompt 1 para Claude 3.7 utilizando modo Thinking y Agent

Como experto en Backend analiza el fichero de @backend para tener una visión más amplia del proyecto

# Prompt 2 para Claude 3.7 utilizando modo Thinking y Agent

Como experto en DevOps crea un pipeline completo de CI/CD en GitHub Actions que debe activarse cuando se hace push a cualquier rama que tenga un Pull Request abierto. El pipeline debe realizar las siguientes operaciones secuenciales:

1. Ejecutar los tests del backend
2. Generar un build del backend
3. Desplegar el backend en una instancia EC2 de AWS

Por favor, crea el archivo de configuración .github/workflows/pipeline-SRG.yml con las siguientes especificaciones:

- El trigger debe ser específicamente "push a una rama con un Pull Request abierto"
- Para los tests: utiliza una configuración estándar para ejecutar tests (npm run test)
- Para el build: genera un artefacto deployable del backend
- Para el despliegue en EC2:
  - Utiliza GitHub Screts para las credenciales de AWS
  - Configura la conexión SSH a la instancia
  - Transfiere los archivos necesarios
  - Reinicia los servicios requeridos

Además, para cada paso principal del pipeline, proporciona un comentario explicativo que documente el propósito de ese paso y cómo funciona.

Asegúrate de que el archivo YAML esté correctamente indentado y siga las mejores prácticas de GitHub Actions.

No des nada por hecho y pregunta lo que sea necesario.

# Prompt 3 para Claude 3.7 utilizando modo Thinking y Agent

Como experto en Devops, podrías revisar este error que ha surgido al momento de hacer el deploy en el GitHub Actions "Run aws-actions/configure-aws-credentials@v4
Error: Input required and not supplied: aws-region". Adicionalmente revisa que otros errores pueden surgir al momento del despliegue para mitigarlos
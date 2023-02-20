# Upload folder to blob storage

Script usado para subir la carpeta `build` de los proyectos React hasta el contenedor _$web_ de una _Storage Account_ en Azure.

# Instalación

```bash
pip install --editable .
```


# Uso

El script busca las credenciales de la _Storage Account_ (connection string) en un archivo de nombre `blob-storage-conn-str` y el contenido a subir en la carpeta `build`. Luego de ubicarse en la carpeta de trabajo con estos 2 requerimientos ejecutar:

```bash
python3 app/main.py
```

Se puede cambiar de manera opcional el archivo de credenciales y la carpeta a subir mediante las flags `--filename` y `directory` respectivamente.

```bash
python3 app/main.py --filename <custom_storage_credencial_file> --directory <custom_directory_to_upload>
```

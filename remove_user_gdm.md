# Remove User from GDM list

Crear un archivo llamado como el usuario que vamos a quitar de la lista.
```bash
sudo nano /var/lib/AccountsService/users/<username>
```

Agregar estas líneas al archivo:
```bash
[User]
Session=
XSession=
Icon=/home/<username>/.face
SystemAccount=true 

[InputSource0]
xkb=latam
```

Para activar de nuevo:
```bash
SystemAccount=false
```



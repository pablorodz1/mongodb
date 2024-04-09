#  Reemplazar Documentos

# Sustituir un documento completo

```m
 db.libros.replaceOne({_id:2},{titulo:'De la tierra a la luna', autor:' Julio Berne', editorial:'Tierra', precio:100})
 ```
 _Dos metodos_

 1.deleteOne
 1. deleteMany

 **Eliminar todo el documento con un id = 2**

```m
  db.libros.deleteOne({_id:2})
 ```

**DeleteMany**

**Eliminar todos los documentos donde la cantidad sea mayor a 150**

 ```m
 db.libros.deleteMany({Cantidad:{$gt:150}})
  ```m
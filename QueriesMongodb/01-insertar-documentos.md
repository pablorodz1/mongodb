# Insertar Documentos

--- 

_Inserta un solo documento_

``` m
db.AlumnosInsertOne(
    {
        nombre."Maximiliano"
    });
```
_Insercion de un documento mas complejo con Array_


```m
db.Alumnos.insertOne(
    {
        nombre: "Rosa",
        edad: 22,
        apellidos:"Vaca",
        aficiones: ["Paracaidismo, "Lectura", "futbol"]
    })
```

_Insercion de Documento con subdocumento_

```m
db.Alumnos.insertOne(
{
 nombre: "Raul",
 edad: 67,
   cv: {
        "Informatica": "Bueno",
        "Marketing": "Malo",
        "Contabilidad": "Medio"
       }
})
```

_Insercion de Documento con Id Personalizado_

```m
db.Alumnos.insertOne({
    _id: 1,
    "Nombre":"Arcadia"
}
)
```

_Insertar multiples Documentos_

```m
 db.Alumnos.insertMany( [ 
{ _id:2, 
   nombre: "Diana", 
  }, 
{ 
    _id:3, 
    nombre: "Flor", edad: 43 
  },
  
{ 
    _id:4, 
    nombre:"Francisco", edad: 34, 
    aficion: "El agua", desgracia: "La ex"
   }]);
```

---

# Operadores de comparacion

| Operador | Descripcion |
| -- | -- |
| $eq | igual |
| $gt | Mayor que |
| $gte | Mayor o igual |
| $in | Buscaar un elemento en un array |
| $lt | Menor que |
| $lte | Menor o igual |
| $ne | Todos los elementos que no sean iguales | 
| $nin | Ninguno de los valores del Arreglo |

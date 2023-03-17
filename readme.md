//Modificar este ejemplo de Persona y pasarlo a Producto con sus respectivos campos...price..stock. No olvidar agregar la mutacion que borra.

//NO hacer front. Solo persistencia en memoria.

//Pegar las querys aqui abajo adaptadas a Productos (ojo que falta el delete!):

//Ejs:
mutation updateUno {
updatePersona(id: "f04fd02885e48c9626ce", datos: {nombre: "messi", edad: 18}) {
id
nombre
edad
}
}

mutation crear {
createPersona(datos: {nombre: "snatiaguito", edad: 35}) {
id
nombre
edad
}
}

query getUno {
getPersona(id: "ae0918d8985c84dcf34a") {
id
nombre
edad
}
}

query todos {
getPersonas {
id
nombre
edad
}
}

query getFiltro {
getPersonas(campo: "nombre", valor: "snatiaguito") {
nombre
id
edad
}
}

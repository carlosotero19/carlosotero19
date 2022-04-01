- 👋 Hi, I’m @carlosotero19
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
carlosotero19/carlosotero19 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


<!DOCTYPE html>
<html>
<head>
    <style>
        #tablero {
            display: inline-block;
            border:5px solid;
        }
        .fila {
            background-color: #999;
            display: table;
        }
        .recuadro {
            width:50px;
            height:50px;
            float:left;
        }
        .fila:nth-child(odd) .recuadro:nth-child(even),
        .fila:nth-child(even) .recuadro:nth-child(odd) {
            background-color: white;
        }
    </style>
</head>
 
<body>
 
    <div id="tablero"></div>
 
</body>
</html>
 
<script>
const tamano=8;
const tablero=document.getElementById("tablero");
for (let i=0; i<tamano; i++) {
 
    // creamos la fila
    let fila=document.createElement("div");
    fila.classList.add("fila")
    for (let j=0; j<tamano; j++) {
 
        // creamos cada elemento de la fila
        let div=document.createElement("div");
        div.classList.add("recuadro")
        fila.appendChild(div);
    }
    tablero.appendChild(fila);
 
}
</script>

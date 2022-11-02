# express_ci_vs2

Pasos para cd 

1 Crear carpeta .github/workflow/cd.yml

[![c1.png](https://i.postimg.cc/vZ4fdk6z/c1.png)](https://postimg.cc/cvNrRDhg)

2 modificar config/config.json to config.js

[![C2.png](https://i.postimg.cc/8zfJYvqX/C2.png)](https://postimg.cc/3k7x4kr2)

3 modificar config/database.js

[![c3.png](https://i.postimg.cc/KjsjqcQy/c3.png)](https://postimg.cc/CnkwdgWv)

4 modificar app.js agregando console.log(process.env.ENV); 

[![c4.png](https://i.postimg.cc/Jzj7JQw8/c4.png)](https://postimg.cc/QFxrZ1xY)

5 crear archivo index.js y agregar // listen on port
const PORT = process.env.PORT || 3001;

app.listen(PORT, () => console.log(`Server running on port ${PORT}`));

[![c5.png](https://i.postimg.cc/KvMmS58T/c5.png)](https://postimg.cc/4msDpVt4)

## Доработка проекта

* Продолжаем улучшать код

1. Создать "универсальную" функцию которая заменит вот этот участок кода в первичном примере
   ```js
   const html = fs.readFileSync("./server/public/index.html") 
   
   ```
   функция **readHTMLPage( name, cb )** должна получить название страницы HTML, найти ее по указанному пути и вернуть используя **callback**
   то есть код который ее вызывает будет выглядеть так
   ```js
   readHTMLPage("index", (content)=>{ console.log(content) })
   ```
2. По тому же принципу сделать функцию которая сможеь загрузить данные и распарсить в виде JSON **readJSONFile( name, cb )**
   ```js
   readJSONFile( "products", (data) => { console.log(data) }) 
   
   ```
   функция **readHTMLPage( name, cb )** должна получить название страницы HTML, найти ее по указанному пути и вернуть используя **callback**
   то есть код который ее вызывает будет выглядеть так
   ```js
   readHTMLPage("index.html", (content)=>{ console.log(content) })
   ```

ПРИМЕЧАНИЕ - для начала сделать простую проверку этих двух функций (test.js который загрузит и выведит данные)

# options-for-html

обнуления
html {
    box-sizing: border-box;
}
*,
*::after,
*::before {
    box-sizing: inherit;
}
h1,
h2,
h3,
h4,
h5,
h6,
p {
    margin: 0;
}
.list {
    list-style: none;
    padding: 0;
    margin: 0;
}
.link {
    text-decoration: none;
    color: inherit;
}
img {
    display: block;
    max-width: 100%;
    height: auto;
}

Для правильного скрытия заголовков используем паттерн -
.visually-hidden {
    position: absolute;
    width: 1px;
    height: 1px;
    margin: -1px;
    border: 0;
    padding: 0;
    white-space: nowrap;
    clip-path: inset(100%);
    clip: rect(0 0 0 0);
    overflow: hidden;
}


Кастомний Checkbox
.label{
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 30px;
  text-align: center;
}

.input{
  position: absolute;
    width: 1px;
    height: 1px;
    margin: -1px;
    border: 0;
    padding: 0;
    clip: rect(0 0 0 0);
    overflow: hidden;
    } 
    
     .svg {
    margin-right: 7px;
    width: 16px;
    height: 15px;
    border: 2px solid var(--main-title-color);
    border-radius: 4px;
    background-color: var(--current-white-color);
    transition-property: background-color, border;
    transition-duration: var(--tr-duration);
    transition-timing-function: var(--timing-function);
}

  .input:checked +  .svg{
  margin-right: 7px;  
  width: 16px;
  height: 16px;
  border-radius: 4px;
  background-color:var(--accent-color);
  border: 2px solid var(--accent-color);
}
   
   
   # options-for-JS
   Підключаєто бібліотеку Lodash для trottle and Dedounnce   -   https://cdnjs.com/libraries/lodash.js
   
   библиотека дял раюотьі с галереей картинок SimpleLightbox, возьмет на себя обработку кликов по изображениям, открытие и закрытие модального окна, а также пролистывание изображений при помощи клавиатуры.    --- https://cdnjs.com/libraries/simplelightbox 
   
   
   
   #настройки для sass
   
   {
    "liveSassCompile.settings.formats": [
        {
            "format": "expanded",
            "extensionName": ".css",
            "savePath": "/css"
        },
        {
            "format": "compressed",
            "extensionName": ".min.css",
            "savePath": "/css"
        }
    ],
    "liveSassCompile.settings.excludeList": [
        "**/node_modules/**",
        ".vscode/**"
    ],
    "liveSassCompile.settings.generateMap": true,
    "liveServer.settings.port": 1235,
    "liveSassCompile.settings.autoprefix": null,

    
}

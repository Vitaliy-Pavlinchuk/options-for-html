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

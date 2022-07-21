# sapui5-in-russian

**Содержание**
- [Что это](#что-это)
- [Как этим пользоваться](#как-этим-пользоваться)
  * [Порядок веток с примерами](#порядок-веток-с-примерами)
- [Подготовка окружения разработчика](#подготовка-окружения-разработчика)
- [FAQ](#faq)
  * [Почему назвал этот репозиторий используя дефисы?](#почему-назвал-этот-репозиторий-используя-дефисы)
  * [Почему каждый шаг примера это отдельная ветка?](#почему-каждый-шаг-примера-это-отдельная-ветка)
## Что это
Цель проекта показать основы работы на фреймворке SAPUI5 с пояснениями на русском языке.

## Как этим пользоваться
Примеры разделены по веткам, причём каждый шаг примера отдельная ветка.
Например, form-controls-1, form-controls-2.

### Порядок веток с примерами
1. form-controls
2. bindings

## Подготовка окружения разработчика
Можно выделить 3 основных способа для написания и запуска кода на SAPUI5:
1. Загрузить на страницу bootstrap скрипт через CDN (Content Deliviry Network).
1. Разработка в облаке.
1. Разработка на базе UI5 CLI.

### 1. Загрузить на страницу bootstrap скрипт через CDN (Content Deliviry Network).
По простому - создать index.html и с помощью тэга <script> добавить скрипт sap-ui-core.js.
 ```html
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title>Quickstart Tutorial</title>
	<script id="sap-ui-bootstrap"
		src="https://openui5.hana.ondemand.com/resources/sap-ui-core.js"
		data-sap-ui-theme="sap_belize"
		data-sap-ui-libs="sap.m"
		data-sap-ui-resourceroots='{"Quickstart": "./"}'
		data-sap-ui-onInit="module:Quickstart/index"
		data-sap-ui-compatVersion="edge"
		data-sap-ui-async="true">
	</script>
</head>
<body class="sapUiBody" id="content"></body>
</html>
 ```
Подробнее: https://sapui5.hana.ondemand.com/1.90.7/#/topic/851bde42e4e1410c96abbe402fa9128c
 
 Для разработки вариант не очень, но подойдёт когда нужно сделать маленький примерчик и выложить на codepen:
 https://codepen.io/vinipolicena/pen/JoegJQ
	
 В таких случаях описывают контролы с помощью JS, но бывает делают это в html: https://codepen.io/JEE42/pen/KaQege.

### 2. Разработка в облаке.
Для этого варианта используют SAP Business Application Studio (BAS) или его предшественика SAP Web IDE.

### 3. Разработка на базе UI5 CLI
Для начала запустим чужой проект, чтобы убедиться что всё работает. Заодно мы увидим пример приложения которые пишут на SAPUI5.

1. Установите ноду и UI5 CLI по инструкции:
https://sap.github.io/ui5-tooling/pages/GettingStarted/
2. Склонируйте и запустите сервер с проектом:
https://github.com/SAP/openui5-sample-app
3. После запуска откройте ссылку: http://localhost:8080/index.html, вы увидите такой непримечательный TODO list.
![image](https://user-images.githubusercontent.com/5730634/179907900-e8c6eb36-2429-4980-972a-2d3c42f8c4bd.png)


## FAQ
### Почему назвал этот репозиторий используя дефисы?
Такой пример предложил визард github.
### Почему каждый шаг примера это отдельная ветка?
Шаги развития примеров - не коммиты и не теги, чтобы можно было исправить рание шаги.

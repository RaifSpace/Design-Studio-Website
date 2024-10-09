•	Используйте reset.css для сброса тех стилей, который браузер задаёт по умолчанию. Создайте отдельный файл reset.css, в который скопируйте все стили указанные на этом сайте. Подключайте его перед основными ваши стилями, то есть самым первым.
https://meyerweb.com/eric/tools/css/reset/
Например:
<link rel="stylesheet" href="./reset.css ">
<link rel="stylesheet" href="./style.css ">

•	Доты в слайдере (images__wrapp) вы можете внутри этого блока создать 3 тега div, задать им ширину и высоту, и округлить их с помощью border-radius: 50%, данный вариант лучше реализовать так, чем использовать svg;

•	В вашем проекте вы не во всех секциях использовали блок контейнер для ограничения ширины контента внутри секций, что не является корректным, так как часть контента на сайте прижата к левой части экрана.
Вот пример реализации проекта с использованием блока контейнера.

Например:
HTML
<header class=”header”>
  <div class=”container”>
    <div class=”header__wrapper”>

<section class=”main-screen”>
  <div class=”container”>
    <div class=”main-screen __wrapper”>

CSS
.container {
  max-width: 1200px;
  margin: 0 auto;
}

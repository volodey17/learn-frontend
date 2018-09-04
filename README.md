# Старт в верстке-сайтов

## Вступление

- Рекомендую использовать редактор Visual Studio Code. В сети много хвалебных отзывов насчет Sublime Text, однако я настоятельно рекомендую использовать VSCode а не Sublime. Я сам продолжительное время использовал Sublime Text-3 и могу сказать, что   на голову выше его. В VSCode многое работает "из коробки", что в Sublime нужно настраивать или это отсутствует. VSCode бесплатен, а Sublime нет. Переход на VSCode скорее всего будет легкий, есть полноценный русский язык редактора, а также как уже говорилось, много работает "из коробки" и не требует настройки. 
- Рекомендую сразу зарегистрироваться на таких ресурсах как: github, codepen, stackoverflow. Зачем например codepen, вот мой там профиль там: https://codepen.io/alexandr-kazakov/ Это подобие небольшого портфолио с кодом, в будущем сможешь показать, что ты что-то умеешь, также если что-нибудь сделаешь полезное, сможешь помочь другим.

## Перед поиском первых заказов на фрилансе

Есть типовые элементы, которые в верстке встречаются особенно часто и к ним нужно быть готовым. Вот они:
1. Адаптивное меню, например такое: https://i.imgur.com/RHhzfFi.png Меню идет с прозрачным фоном, над секцией с картинкой-фоном. При скролле страницы, меню фиксированное(всегда наверху), следовательно, при скролле страницы у меню появляется темный фон, также само меню становится меньше(по высоте, логотип и любой текст). На мобильных часть меню скрывается и появляется кнопка-гамбургер, при клике на кнопку-габмергер - меню появляется. Нужно уметь делать два базовых типа появления меню: горизонтальное(выезжает вниз), например: https://erweb.ru/layout/toy-sale/ и вертикальное, что появляется справа или слева, например: https://erweb.ru/layout/miele/

## Кроссбраузерность

Здесь я постараюсь писать наиболее популярные особенности в кроссбраузерности о которых нужно знать:
1. Для любого input лучше всего писать font-size: 16px и больше(главное не меньше). Если написать меньше, то в iOS идет автоматический zoom страницы. Подробнее: https://stackoverflow.com/q/2989263/7460038
2. Стоит использовать normalize.css, а если нет, то нужно помнить про свойство: -webkit-appearance. Суть здесь следующая, iOS изменяет внешний вид у некоторых элементов, типа [type='submit'] Подробнее: https://stackoverflow.com/questions/5449412/styling-input-buttons-for-ipad-and-iphone 
* Рекомендую стараться регулярно скачивать свежую версию normalize с оф. сайта, так как ее периодически обновляют(старый хлам убирают).
* Если вы используете Bootstra-4(полную версию), отдельно normalize подключать не нужно, он уже туда включен.

## Современные возможности

Здесь постараюсь писать, что нужно использовать в настоящее момент, чтобы не тратить время на изучение устаревших технологий:
1. Используйте flex и не используйте float. Раньше, в эпоху Bootstra-3, для построения сетки использовались float-ы, так как flex-ы старые браузеры не поддерживали. Можно увидеть массовое использование float-ов в верстке, в разных там учебниках/видео/курсах, это вчерашний день. С момента прихода Bootstrap-4 преимущественно используются flex-ы. Про float-ы нужно знать и иногда можно их применять, но не более того.



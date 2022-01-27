# Тестовое задание для WordPress Fullstack Developer
<img width="200" src="https://raw.githubusercontent.com/wowvendor/wowvendor-junior-test/97bf30dc6a091261bd6fc6409e9c8e2791c3d745/images/donut.svg">\
\
Для выполнения тестового задания необходимо склонировать данный репозиторий на локальную машину. \
В качестве результата задания принимается ссылка на публичный репозиторий в Github

## На выполнение тестового задания отводится 2 дня

## Дано:

Приложение мини-игра. Целью игры является добежать до финиша, не столкнувшись с препятствием.\
В приложении реализованы основные методы управления персонажем: ```run, stop, jump```;

## Задачи:
1. На базе приложения создать WordPress-плагин;
2. В плагине добавить возможность отображать мини-игру на определённой странице (page) или странице записи (post);
3. Сверстать игру на странице в соответствии с макетом: https://www.figma.com/file/7clxADgstjr2n9vq3BN8cr/%D0%A2%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D0%BE%D0%B5-%D0%97%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-(Frontend)?node-id=7%3A16322 . Адаптивная вёрстка для блока с игрой не нужна;
4. При открытии страницы, поверх мини-игры появляется всплывающее окно с предложением начать игру;
5. У игры есть два режима: ручной и автоматический;
6. В ручном режиме у игры появляются кнопки управления: S, D и Space;
7. В автоматическом режиме кнопки управления не появляются, а пончик проходит игру автоматически (автоматически бегает и перепрыгивает через препятствие);
8. Переключить режим игры можно в попапе настроек;
9. Написать PHP скрипт, принимающий результаты забега и записывающий их в базу данных WordPress;
10. Отправлять результаты забега каждый раз, когда персонаж доходит до финиша или спотыкается о препятствие;
11. Под блоком с игрой выводится статистика игр, упорядоченная по времени;
12. Также сводная статистика по играм выводится в попапе настроек.

### Результаты забега:

1. Позиция препятствия;
2. Время забега;
3. Дистанция на которой персонаж совершил прыжок;
4. Размер препятствия;
5. Результат забега (Успех или Провал).


### Получение данных и методы управления:

#### Управление персонажем:
```js
    window.character.run(); 
    window.character.stop(); 
    window.character.jump(); 
```

#### Публичные свойства:
```js
    window.terrain.rockPosition; 
    window.terrain.rockSize;
    window.character.characterPosition;
```
### Результаты работы:
Публичный репозиторий Github, содержащий:
1. Репозиторий с вашим плагином.

### Необязательное условие:
1. Вы можете представить полноценный репозиторий с docker-контейнером WordPress, в котором установлен ваш плагин;
2. В таком случае в корень репозитория следует также положить дамп базы данных.

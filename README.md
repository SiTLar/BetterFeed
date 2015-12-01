# BetterFeed

![License](https://img.shields.io/badge/license-MIT-blue.svg)

Это браузерный юзерскрипт, который добавляет некоторые удобства к [FreeFeed](https://freefeed.net/)-у.

## Как установить?

FreeFeed поддерживает BetterFeed, но по умолчанию он выключен. Чтобы его включить, надо зайти в [настройки своего аккаунта](https://freefeed.net/settings), 
поставить в разделе _Add-ons_ галочку _Enable BetterFeed_ и нажать _Apply_. 

BetterFeed обновляется автоматически, обновления проверяются один раз в сутки. Обновиться можно и вручную, для этого в настройках 
есть кнопка «Проверить обновления». Ссылка на настройки BetterFeed находится в самом низу правой колонки FreeFeed-а.

## Что он умеет?

Каждая из перечисленных ниже функций может быть отключена или включена в настройках BetterFeed-а.

 * Заменяет креативные ники на скучные логины;
 * Если первое слишком радикально, то можно после юзернейма в скобках показывать логин пользователя;
 * Показывает приложенные к постам картинки в красивых лайтбоксах;
 * Показывает ссылку 'Add comment' под комментариями к посту (в тех случаях, когда её на ставит сам FreeFeed);
 * Разноцветные облачка у комментариев (оранжевые у вас, тёмно-серые у автора треда, голубые у ваших френдов, светло-серые у ваших читателей);
 * При клике на облачко в поле комментария вставляется @логин или ^^^ при клике с Ctrl/Cmd;
 * "@логины" в тексте становятся ссылками;
 * При наведении на "@логин" или "^^^"/"↑↑↑" в комментарии, подсвечиваются соответствующие комментарии;
 * Вместо анимированных гифовых превьюшек показывается стоп-кадр;
 * В общей ленте постов показывается, чей комментарий или лайк принесли в ленту этот пост (если пост не от френда), также можно скрывать посты не от френдов или от определённых пользователей;
 * Можно скрывать комментарии от определённых пользователей;
 * Облачко рядом с комментарием заменяется на юзерпик автора. Если включена настройка «разноцветные облачка», то под юзерпиком показывается полоска соответствующего цвета;
 * Если в посте есть ссылки и нет аттачей, то после тела поста добавляется краткое превью ссылки (используется сервис http://embed.ly/code). Можно отключить показ превью для конкретной ссылки, для этого перед ссылкой без пробела надо поставить восклицательный знак: !https://…;
 * Для аттачей-документов (pdf, ppt, doc(x), xls(x), txt) показывается превью;
 * При наведении мыши на пользователя, показывается окошко с краткой информацией о нём и возможностью подписаться/отписаться, захайдить/расхайдить, забанить/разбанить;
 * При наведении мыши на комментарий показывается его порядковый номер в посте;
 * В текстах постов и комментариев можно использовать переводы строк (вводятся через `Shift+Enter`);
 * Слишком длинные посты и комментарии сворачиваются под кнопку «Read more...»;
 * Сообщения-директы выделяются серым фоном;
 * В постах и комментариях показываются emoji (вводятся в формате `:emoji:` или как unicode-символы);
 * Ссылка на собственный профиль показывается как скриннейм/юзернейм, а не как *You*;
 * Перед удалением поста или комментария запрашивается подтверждение;
 * В списке подписчиков группы на иконке администратора рисуется коронка, в списках подписок и подписчиков текущего пользователя отмечаются взаимные френды;
 * У последовательных комментариев одного автора скрывается иконка/юзерпик комментария;
 * Для постов и комментариев старше суток выводится не относительное, а абсолютное время;
 * При выборе адресатов директ-сообщения выводится предупреждение, если выбраны как пользователи так и фиды/группы;
 * Можно задавать описание для собственного фида или групп, в которых вы админ. Описание показывается на странице фида, вверху;
 * Быстрое переключение между аккаунтами без ввода пароля;
 * Уведомления о новых или обновлённых (прокомментированных) директ-сообщениях;
 * Иконки юзеров/групп в селекторе адресатов поста;
 
 * Пока всё.
 
## Почему юзерскрипт, а не вклад в код самого FreeFeed-а?

К сожалению, мне сложно разобраться в существующем коде FreeFeed-а. Это, конечно, характеризует скорее меня, чем код, но тем не менее. 
Мне _быстрее_ и _удобнее_ написать быстрый фикс поверх сайта, чем понять всю его архитектуру изнутри. Если результат одинаков, то зачем платить больше?:)
 
К тому же, мне в принципе кажется хорошей идея «твиков» поверх существующего сайта. Создатели сайта могут сфокусироваться на действительно важных вещах -- оптимизации 
движка и реализации функций, которые не сводятся к интерфейсу. В то время как интерфейс можно быстро фиксить такими вот скриптами. Опять же, это неплохая обкатка фич, 
которые потом могут перекочевать в основной код.

 
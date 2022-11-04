Galada - Легкая и Простая тема для личного блога
======
Galada — легкая и простая тема для Jekyll. Темные цвета, придают ему особый изысканный вид. Тщательный подход к дизайну и возможностям делает его идеальным решением для личного блога.

* * *

Оглавление
-----------------
*   [Features](#features)
*   [Demo](#demo)
*   [Deployment](#deployment)
*   [Posts](#posts)
*   [Disqus Comments](#DisqusComments)
*   [Instagram](#instagram)
*   [Google Analytics](#GoogleAnalytics)
*   [Update favicon](#UpdateFavicon)
*   [Credits](#Credits)
*   [Support](#Support)

* * *

### Features

* 100% отзывчивая и чистая тема

* Оптимизирован для мобильных устройств

* Минималистичный дизайн

* Действительный код HTML5

* Обмен сообщениями

* Форма подписки

* Поддерживает комментарии Disqus

* Лента Instagram

* Иконки Ионикон

* Гугл шрифты

* * *

### Demo

Check the theme in action [Demo](https://artemsheludko.github.io/galada/)

![Main page preview](https://github.com/artemsheludko/galada/blob/master/img/galada-main-page.jpg?raw=true)

The post page would look like this:

![Post page preview](https://github.com/artemsheludko/galada/blob/master/img/galada-post.jpg?raw=true)

* * *

### Deployment

Чтобы запустить тему локально, перейдите в каталог темы и запустите «bundle install», чтобы установить зависимости, затем запустите «jekyll serve» или «bundle exec jekyll serve», чтобы запустить сервер Jekyll.

Я бы рекомендовал проверить страницу [Методы развертывания] (https://jekyllrb.com/docs/deployment-methods/) на веб-сайте Jekyll.

* * *

### Posts

Чтобы создать новый пост, вы можете создать новый файл уценки в каталоге \_posts, следуя [рекомендуемой файловой структуре](https://jekyllrb.com/docs/posts/#creating-post-files).

      ---
      layout: post
      title: Premiere on Broadway
      date: 2018-08-23 16:04:00 +0300
      image: 03.jpg
      tags: [Rest]
      ---
          

Вы можете установить теги и изображение поста.

Добавьте изображения постов в каталог **/img/**.

Для тегов старайтесь не добавлять пробел между двумя словами, например, «Ruby on Rails», может быть что-то вроде ( «ruby-on-rails», «Ruby_on_Rails» или «Ruby-on-Rails»).
* * *

### Disqus Comments

Тема Galada поставляется с включенными комментариями Disqus.

Откройте файл _config.yml и измените значение mr-brown в строке 26 на свое [короткое имя учетной записи Disqus] (https://help.disqus.com/customer/portal/articles/466208).

       Раздел комментариев (Disqus)
       disqus-identifier: mr-brown \# Добавьте свое короткое имя для комментария Disqus. Например, мистер Браун
          

Это все, что вам нужно для настройки Disqus со стороны темы. Если у вас возникнут какие-либо проблемы, связанные с этим, комментарии не могут быть загружены. Во-первых, убедитесь, что вы [зарегистрировали свой веб-сайт в Disqus (шаг 1)](https://help.disqus.com/customer/portal/articles/466182-publisher-quick-start-guide).

А также проверьте [Руководство по устранению неполадок Disqus](https://help.disqus.com/customer/portal/articles/472007-i-m-receive-the-message-%22we-were-unable-to-load-disqus-%22 ), если у вас все еще есть проблемы.
* * *

### Instagram
Канал Instagram работает с использованием [Instafeed.js](http://instafeedjs.com/) для показа фотографий.

Во-первых, вам нужно будет получить `userId` и `accessToken` вашей учетной записи со следующих URL-адресов:

* идентификатор пользователя: [smashballoon.com/instagram-feed/find-instagram-user-id](https://smashballoon.com/instagram-feed/find-instagram-user-id/)
* accessToken: [instagram.pixelunion.net](http://instagram.pixelunion.net/)

Во-вторых, откройте файл js/common.js и замените значения userId и accessToken.

            var instagramFeed = new Instafeed({
              get: 'user',
              limit: 6,
              resolution: 'standard_resolution',
              userId: '8987997106',
              accessToken: '8987997106.924f677.8555ecbd52584f41b9b22ec1a16dafb9',
              template: ''
            });
          

В-третьих, откройте файл _config.yml и замените значение instafeed: false на instafeed: true.

            \# Лента Instagram
            instafeed: false \# Чтобы включить instafeed, используйте значение true. Для выключения используйте значение false.

* * *

### Google Analytics

Чтобы интегрировать Google Analytics, откройте файл _config.yml и добавьте свой идентификатор Google Analytics.

     \# Гугл Аналитика
     google-analytics: \# Добавьте свой идентификатор. Например UA-99631805-1

* * *

### Update favicon

Вы можете найти текущий значок (favicon.ico) в корневом каталоге темы, просто замените его новым значком.

* * *

### Credits

Я использовал следующие сценарии, шрифты или другие файлы, указанные в списке.

*   [Google Fonts](https://fonts.google.com/specimen/Nunito) (Nunito, Sans Serif).
*   [Ionicons Icons](https://ionicons.com/)
*   [FitVids.js](http://fitvidsjs.com/)
*   [Instafeed.js](http://instafeedjs.com/)
*   [jQuery.com](https://jquery.com/)
*   [Wait For Images](https://github.com/alexanderdickson/waitForImages)
*   Preview Images form [unsplash.com](https://unsplash.com/), [pexels.com](https://www.pexels.com/)

* * *
### License

Mit License

* * *

### Support

<p>If you like the themes that I create you can become my sponsor on <a href="https://www.patreon.com/artemsheludko" target="_blank">Patreon</a>.
<p align="center"><b>Thank you for your support ❤️</b></p>

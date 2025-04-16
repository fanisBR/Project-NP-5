Команды в shell

управление py.startapp новое приложение
py manage.py оболочка
py manage.py совершайте миграции
py manage.py миграция
из newapp.импорт моделей *

user1 = User.objects.create(имя_пользователя='Майк', имя='Фрэнк')

Author.objects.create(authorUser=user1)

Категория.объекты.создать(authorUser=user2)

Пользователь2 = User.objects.create(имя_пользователя='Семён', имя='Бер')
Author.objects.create(authorUser=user2)
Категория.объекты.создать(name='ЭТО')
Категория.объекты.создать(name='Образование')
Post.objects.create(автор=Author.objects.get(AuthorUser=User.objects.get(имя_пользователя="Майк")), тип_категории="NW", заголовок="заголовок", текст="какой-то текст")
p1 = Post.objects.get(pk=1)
c1 = Category.objects.get(название = «IT»)
p1.postCategory.добавить(c1)
Комментарий. объекты. создать (комментарий. пользователь = Пользователь. объекты. получить (имя пользователя = «Майк»), комментарий. пост = Пост. объекты. получить (идентификатор = 1), текст = «комментарий. текст 1»)
Post.objects.get(pk=1).like()
Комментарий.объекты.get(pk=1).нравится()
Автор. объекты. получить (AuthorUser = Пользователь. объекты. получить (имя_пользователя = «Майк»)). обновить_рейтинг()
a = Author.objects.get(AuthorUser = User.objects.get(имя_пользователя = 'Семён'))
a.Оценивающий автор
Автор. объекты. получить (AuthorUser = Пользователь. объекты. получить (имя пользователя = «Майк»)). рейтинг автора
best = Author.objects.all().order_by('-ratingAuthor').values('authorUser', 'ratingAuthor')[0]
печать (лучшая)

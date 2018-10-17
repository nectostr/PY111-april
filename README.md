Задания для группы PY101-october
=

**Как пользоваться данным репозиторием?**

- Сделайте форк данного репозитория, нажав кнопку "Fork" наверху страницы
- Склонируйте репозиторий на ваше устройство
- Присоедините вашу ветку к этому репозиторию, выполнив следующую команду:
 
```
git remote add -t master python https://github.com/maybe-hello-world/PY101-october
```

Вы можете посмотреть список подключенных удаленных источников с помощью команды `git remote show`. Результат должен быть примерно следующим:

```
# git remote show

python
origin
```

**Выполнение заданий**

Перед тем, как начать, заберите изменения из моего репозитория:

```
git pull python master
```

Если версия вашего репозитория более старая, нежели версия ветки master данного репозитория, вам необходимо сделать "rebase" изменений из данного репозитория в ваш мастер.
Делается это следующим образом:

```
git rebase python/master master
```

Далее отправьте изменения из вашего локального репозитория в ваш удаленный:

```
git push origin master
```

Затем выполните следующий шаг, чтобы переключиться к вашей личной ветке:

```
git checkout <PRIVATE_BRANCH_NAME>
```

Затем создайте новую ветку для выполнения задания:

```
git checkout -b <TASK_BRANCH>
```

Откройте вашу любимую IDE и напишите код для решения задачи, после чего не забудьте сделать коммит.

```
git add .
git commit
```

Когда вы сочтете, что ваше задание решено, вы должны слить изменения из ветки с заданием в вашу приватную ветку:

```
git checkout <PRIVATE_BRANCH_NAME>
git rebase <TASK_BRANCH>
```

Теперь вы можете отправить ваши изменения в ваш собственный удаленный репозиторий:
 
```
git push origin <PRIVATE_BRANCH_NAME>
```

Когда ваши изменения отправились в ваш собственный форк, вам необходимо сделать пулл-реквест. Хорошим тоном будет добавить метку "Excercise" к вашему пулл-реквесту для того, чтобы его легко можно было опознать.

**Как помочь данному репозиторию**

Вы можете помочь данному репозиторию, создавая или исправляя тесты для заданий. Создайте тест и отправьте пулл-реквест с пометкой "Test", чтобы я обратил на это внимание.

# Console

pwd – показать рабочую папку

cd «путь» - сменить директорию

cd .. – переход на уровень выше

ls [-a] – отобразить содержимое директории [отображает скрытые папки]

touch «имя файла» - создает новый файл

mkdir «имя папки» - создает дерикторию

mkdir -p «путь к папке» - создает структуру директорий

cd «что копируем_1, что копируем_2, ..» «путь куда» - копирует файлы

cat «имя файла» – чтение и печать текстовых файлов в консоль;

rm «имя файла» - удалить файл безвозвратно;

rm -r «имя папки» - удалить папку и все что внутри;

rmdir «имя папки» - удалить пустую папку;

«команда 1» && «команда 2» - выполнение нескольких команд в одну строчку

_Tab_ - автозаполнение команд и пути



# GIT

git init – инициализирует git репозиторий 

rm -rf .git - удалить папку git (разгитить)

git status – показывает текущее состояние репозитория

git add «имя файла» - подготовить файл к сохранению

git add --all – подготовить к сохранению все файлы в директории 

git add . – подготовить к сохранению всю текущую директорию

git commit -m «сообщение» - выполнить коммит

git log – посмотреть историю коммитов

git log --oneline - получить сокращенный лог

ls -la .ssh/  - вывести список созданных ключей ssh

ssh-keygen -t «id_rsa[i]» -C «email для GitHub аккаунта» – генерация ssh-пары ключей

id_rsa = [ed25519, rsa -b 4096] 

clip < ~/.ssh/id_ed25519.pub – скопировать содержимое ключа в буфер

ssh -T git@github.com – проверить правильность ключа после добавления в github

git remote add origin git@github.com:[логин]/[имя проекта].git - привязать удаленный репозиторий к локальному

git remote -v – проверка, что репозитории связаны

git push -u origin master – отправить изменения на удаленный репозиторий


# Хеш - идентификатор коммита

- Хеширование - преобразование набора данных для получения их "отпечатка";
- Хеш коммита получается с помощью алгоритма SHA-1;
- Хеш состоит из цифр 0-9 и латинских букв A-F;
- Если дважды получить хеш для одного набора данных, результат будет одинаковый;
- Если изменить что-то в исходных данных, хеш измениться;
- Хеш - основной идентификатор коммита, позволяет узнать автора, дату и содержимое закоммиченных файлов;
- Хеши и таблицу хеш информацию о коммите Git сохраняет в служебных файлах в папке .git.

# Исследуем лог

- Лог содержит описание коммита: хеш, автора, дата, сообщение;
- Сокращенный лог помогает быстро найти нужный коммит среди множества;
- Уникальная длина сокращенных хешей помогает идентифицировать коммит.




 


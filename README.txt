РУЛЕТКА — APK для Android (игра открывается горизонтально, на весь экран)

СПОСОБ 1. Android Studio на вашем компьютере (без интернет-сервисов)
 1. Скачайте Android Studio: developer.android.com/studio. Установка обычная (Next -> Next -> Finish).
 2. Распакуйте этот архив. Запустите Android Studio -> Open -> выберите папку Ruletka-Android
    (в которой лежит файл settings.gradle).
 3. Подождите, пока внизу закончится Gradle sync (первый раз 5-15 минут, нужен интернет).
    Если студия просит установить Android SDK 34 или принять лицензии — нажимайте Install / Accept.
    Если предлагает обновить Gradle или плагин — выберите "Don't remind me" / Skip.
 4. Меню Build -> Build Bundle(s) / APK(s) -> Build APK(s).
 5. Справа внизу появится "APK(s) generated successfully" -> ссылка locate.
    Файл лежит здесь: app\build\outputs\apk\debug\app-debug.apk

СПОСОБ 2. Сборка в облаке GitHub (ничего не нужно ставить на ПК)
 1. github.com -> New repository (Public) -> uploading an existing file.
 2. Перетащите ВСЁ содержимое папки Ruletka-Android (settings.gradle, app, gradle и т.д.).
    Если скрытая папка .github не загрузилась: Add file -> Create new file, имя
    .github/workflows/android.yml, вставьте текст из одноимённого файла. Commit changes.
 3. Вкладка Actions -> дождитесь зелёной галочки (3-8 минут).
 4. Откройте запуск -> внизу Artifacts -> Ruletka-apk -> скачайте. Внутри app-debug.apk.

КАК УСТАНОВИТЬ APK (любому человеку на Android)
 1. Отправьте файл app-debug.apk в Telegram, на почту, в облако или по USB.
    (Если мессенджер не пропускает .apk — упакуйте в ZIP.)
 2. На телефоне скачайте файл и нажмите на него.
 3. Android спросит разрешение "Установка из неизвестных источников" для приложения, через
    которое вы открыли файл (Telegram, Chrome, Файлы). Откройте Настройки и включите разрешение.
 4. Нажмите "Установить". Если Google Play Protect пишет "Приложение не проверено" — нажмите
    "Подробнее" -> "Всё равно установить".
 5. Иконка "Рулетка" появится в меню приложений. Телефон держите горизонтально.

iPhone не открывает APK. Для iPhone используйте архив Ruletka-phone (иконка на экран "Домой").

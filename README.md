# Telegram_Crawler
1. install everything you need from the file "requirements.txt "
2. to set up your "tg_parser_project\utils\config.py " API_ID, API_HASH to log in to the telegram account, you need to go to the website first "https://my.telegram.org /" go to the "API development tools" tab, fill in all the necessary information, and at the end we get "App api_id:" "App api_hash:"
3. Steps to recreate the chrome_profile:

    1. Delete the old profile 
       Open PowerShell and enter:

       Remove-Item -Recurse -Force "E:\Telegram_crawler\chrome_profile"

       (if VSCode is busy, close it first so that Chrome is not in the background)

    2. Launch Chrome manually with a new profile:

       Start-Process "chrome.exe" -ArgumentList "--user-data-dir=E:\Telegram_crawler\chrome_profile", "--profile-directory=Default"

       This will open a clean Chrome bound to E:\Telegram_crawler\chrome_profile

    3. In a new window:
       Go to https://web.telegram.org/k

       Log in via Telegram

       Go to https://tgstat.ru

       Log in via the Telegram button (registration takes place through their tg bot, you just need to click on the "Log in" button)

       Make sure that you have logged in and the site remembers you (after you are sure, close the browser)

4. Run the parser code "python main.py "

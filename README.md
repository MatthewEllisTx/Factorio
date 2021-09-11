Not much going on here, this is just our factorio world. Feel free to download it and make fun of how bad it is ig

Add this to bash.bashrc

    # factorio pull
    factorio-pull(){
        cd "C:\\Users\\{{account_name}}\\AppData\\Roaming\\Factorio\\saves"
        git pull origin main
        ./start-watching.bat
    }

When the command is run it will update the local world with github. When the world is saved it will automatically push

Found when_changed.exe [here](https://github.com/benblamey/when_changed). Only change to "fix" it was changing console.ReadKey(true) to console.read(), because it doesn't like being run in gitbash

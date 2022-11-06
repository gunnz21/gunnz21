- 👋 Hi, I’m @gunnz21
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

#GUI Template#

Function MainMenu {
    cls
    write-host "test"
    Write-Host ""
    Write-Host "1.) Menu 1"
    Write-Host "2.) Menu 2"
    Write-Host ""
    Write-Host "Q: quit"
    Write-Host ""
    $Sel = Read-Host "Selection"
    MenuSelect
}

FUNCTION MenuSelect {
    cls
    Write-Host "Choice is: $Sel"
    switch ($Sel){
        1 {"It is one."}
        2 {"It is two."}
        3 {"It is three."}
        4 {"It is four."}
        Default {
            "No matches"
            Pause
            MainMenu
        }
    }
}



MainMenu


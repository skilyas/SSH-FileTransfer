# SSH-FileTransfer

forfiles /p "%1" /s /d -%2 /c "cmd /c del /s /q @file"

forfiles -p "%1" -d -%2 -c "cmd /c if @isdir==TRUE rd /s /q @path"

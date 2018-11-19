search folder and sub folder for specific file name and delete
create empty file with notepad
put
for /f "delims=" %%F in ('dir /b /ad /s "drive:/dir/subdir"') do del "%%F\filename.exe"
save as d.bat
run it.
sample 1 : delete all "new folder.exe" from e drive
for /f "delims=" %%F in ('dir /b /ad /s "e:"') do del "%%F\new folder.exe"
sample 2 : delete all "newfolder.exe" from e:\f1
for /f "delims=" %%F in ('dir /b /ad /s "e:\f1"') do del "%%F\newfolder.exe"

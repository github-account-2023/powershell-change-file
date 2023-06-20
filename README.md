```
$filePath = 'C:\path\to\file.bin'
$fileBytes = [System.IO.File]::ReadAllBytes($filePath)
$fileBytes[11] = 0
[System.IO.File]::WriteAllBytes($filePath, $fileBytes)
```

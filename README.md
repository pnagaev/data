# data
Файлы с генерированными данными находятся по ссылке
[Папка с файлами](https://disk.yandex.ru/d/WfbNEm2ZqPky8Q)

Цифра в названии файла показывает сколько записей находится в файле.

![image](https://github.com/pnagaev/data/assets/15208026/43c2c7b4-d423-4a15-9d95-e33b9eeb279e)(https://disk.yandex.ru/d/WfbNEm2ZqPky8Q)


Сгенерированные данные были получены с сайта [https://randomdatatools.ru](https://randomdatatools.ru) по 100 записей

```powershell
$MyDataPath="c:\Scripts\Data\mydata-sorted1.txt"

$b=Invoke-WebRequest("https://api.randomdatatools.ru/?count=100") |ConvertFrom-Json 

$b| Export-Csv -Path $MyDataPath -Encoding UTF8 -Delimiter "`t" -Append
```

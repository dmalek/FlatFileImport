# FlatFileImport	
Flat File Import (FFI)

FFI is CLI tool for importing large data from CSV to SQL Server.


Create new project:
`
FFI.exe --new newProject.json
`

Load and execute  project:
`
FFI.exe --run newProject.json
`

Project file (json):
```
{
  "DestinationConnectionString": null,
  "ImportFilePath": null,
  "ImportFolderPath": "C:\\Export\\",
  "ImportFilePattern": "*",
  "TruncateTable": false,
  "BatchSize": 50000,
  "NullString": "\\N",
  "Separator": "\t",
  "LineTrimStart": "",
  "LineTrimEnd": "",
  "FirstLine": 1,
  "TrimValues": false,
  "NewLineValue": "\\r\\n",
  "BooleanTrueValue": "t",
  "BooleanFalseValue": "f",
  "LogFilePath": null
}
```


CSV file name and structure must mach table name and structure. 

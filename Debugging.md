//xxxxxxxxxxxxxx
Vs code ile iki yöntem bulunmakta.

Extensionlardan "debugger for chrome" yüklenir

vsconde lunch json dosyasına

fff

````
{
  // Use IntelliSense to learn about possible attributes.
  // Hover to view descriptions of existing attributes.
  // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
  "version": "0.2.0",
  "configurations": [
    {
      "type": "chrome",
      "request": "attach",
      "name": "Launch Chrome against localhost",
      "url": "http://localhost:3000",
      "webRoot": "${workspaceFolder}"
    },
    {
      "name": "Attach to url with files served from ./out",
      "type": "chrome",
      "request": "attach",
      "port": 9222,
      "url": "http://localhost:3000",
      "webRoot": "${workspaceFolder}/out"
    }
  ]
}
````
#### url nin server portu olmasına dikkat et. Varsayılan olarakr  8080 gelir onu değiştir

### 1.Launch Chrome against localhost
Bu yöntemde yeni bir chrome yeni bir form olarak açılır.
Tanımlı kullanıcı vs sıfırlanır.

### 2.Attach to url with files served
Chrome için masaustüne kısayol oluştur ve kısayolun yolunu aşadaki şekilde güncelle.
"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --remote-debugging-port=9222

Bu kısayoldan chrome açıldıktan sonra debug çalıştırılır.
Bu yöntemde var olan browser üzerinden 9222 portu üzerinden debug yapılır







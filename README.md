# google-app-script  


## clasp  ( for work in vscode editor )
[google/clasp on Github](https://github.com/google/clasp)  

### ✨ Install global `clasp` first time  
```
sudo npm install -g @google/clasp

```  

Then enable the Google Apps Script API: [https://script.google.com/home/usersettings](https://script.google.com/home/usersettings)   

> Set to `ON`  

![Enable Apps Script API](https://user-images.githubusercontent.com/744973/54870967-a9135780-4d6a-11e9-991c-9f57a508bdf0.gif)  

## Login to use clasp – The Apps Script CLI  

```
clasp login
```
confirm your email and allow all  

## Usage  

- create package.json  
```
npm init -y
```  

## ✨ install package for auto complete code  
`docs > typescript.md`  

```
npm i -D @types/google-apps-script
```  

- create some files  
```
touch LICENSE .gitignore README.md
```  

## ✨ Clone project to vscode
- create `src` folder in vscode

- find project Id in Apps Script browser project

https://github.com/user-attachments/assets/66da7190-1270-42fa-b3d6-0560401ca6d4

- clone app script project by ID: into `src` folder
In terminal
```
clasp clone `<Id Project>` --rootDir src
```  

- move `.clasp.json` to root
In terminal  
```
mv src/.clasp.json .
```  

## push to Apps Script browser  
In terminal  
```
clasp push
```

## pull to local machine  
In terminal  
```
clasp pull
```  

## ✨ push and watch changes  
In terminal
```
clasp push -w
```  

## check files list that push to Apps Script browser  
In terminal  
```
clasp status
```
## logout  
In terminal  
```
clasp logout
```

## Open the Apps Script browser on script.google.com:  
In terminal
```
clasp open
```

> 🎉 🎉 🎉 We can update from vscode editor and push it, refresh web page to see update on web browser


---  


## Resource  
- [Google Clasp :](https://github.com/google/clasp)  
- [Develop Google Apps Script Locally in VSCode using CLASP : On Youtube ](https://www.youtube.com/watch?v=lwxiEB-Mnys)
- [ครูอภิวัฒน์"สอนสร้างสื่อ : On Youtube"](https://www.youtube.com/@KruApiwat/playlists)  

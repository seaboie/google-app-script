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

## ✨ get auto complete code  


- create some files  
```
touch LICENSE .gitignore README.md
```  

## ✨ Clone project to vscode
- create `src` folder in vscode

- find project Id in Apps Script browser project  

<video  controls>
  <source src="https://raw.githubusercontent.com/seaboie/images/main/images/vdo/getId.mp4
  " type="video/mp4">
  Your browser does not support the video tag.
</video>

- clone app script project by ID: into `src` folder
```
clasp clone `<Id Project>` --rootDir src
```  

- move `.clasp.json` to root  
```
mv src/.clasp.json .
```  

## push to Apps Script browser  
```
clasp push
```

## pull to local machine  
```
clasp pull
```  

## ✨ push and watch changes  
```
clasp push -w
```  

## check files list that push to Apps Script browser
```
clasp status
```
## logout  
```
clasp logout
```

## Open the Apps Script browser on script.google.com:
```
clasp open
```

> 🎉 🎉 🎉 We can update from vscode editor and push it, refresh web page to see update on web browser


---  


## Resource  
- [Google Clasp :](https://github.com/google/clasp)  
- [Develop Google Apps Script Locally in VSCode using CLASP : On Youtube ](https://www.youtube.com/watch?v=lwxiEB-Mnys)
- [ครูอภิวัฒน์"สอนสร้างสื่อ : On Youtube"](https://www.youtube.com/@KruApiwat/playlists)  

# google-app-script  

### Watch on Youtube  
📺  📺  📺 [Youtube : Create new apps script project in vscode use Clasp](https://youtu.be/UCjwkfuwJj0)  
📺  📺  📺 [Youtube : Clone google apps script to VSCode use Clasp](https://youtu.be/LU-x0t22Onw)  

## Google Workspace  
### [clasp docs](https://developers.google.com/apps-script/guides/clasp)  

## clasp  ( for work in vscode editor )
[google/clasp on Github](https://github.com/google/clasp)  

### ✨ Install global `clasp` first time  
> for Mac use `sudo`
```
sudo npm install -g @google/clasp

```  

Then enable the Google Apps Script API: [https://script.google.com/home/usersettings](https://script.google.com/home/usersettings)   

> Set to `ON`  

![Enable Apps Script API](https://user-images.githubusercontent.com/744973/54870967-a9135780-4d6a-11e9-991c-9f57a508bdf0.gif)  

## Login to use clasp – The Apps Script CLI  
This command logs in and authorizes management of your Google account's Apps Script projects. Once it is run, you are asked to sign into a Google account where your Apps Script projects are stored.

```
clasp login
```
confirm your email and allow all  

---  
---  

## Create new basic Directory Structure in VSCode use `npm`  

- create new directory and name it  

```bash
mkdir example-project
```  

- `cd` to new directory  

```bash
cd example-project
```  

- create package.json  
```
npm init -y
```  

#### 🛠️ install package for auto complete code  

```
npm i -D @types/google-apps-script
```  

- create `src` directory  
```bash
mkdir src
```  

- create some files  
```
touch LICENSE .gitignore README.md
```  

```text
Project
├── ./src
├── LICENSE
├── package.json
└── README.md
```  

---   
---  
---  
---  


## ✨ 1. New project with clasp  

<a href="#create-new-basic-directory-structure-in-vscode-use-npm">Create new Project</a>  

```text
Project
├── ./src
├── LICENSE
├── package.json
└── README.md
```  


We can create the new Apps Script project using `clasp create` with Project name `--title <project name>` :  

`Interminal`  

```bash
clasp create --title "ชื่อโครงการใหม่" --rootDir src
```
`Enter`  

```bash
# interminal


% clasp create --title "ชื่อโครงการใหม่"
? Create which script? 
  standalone 
  docs 
❯ sheets 
  slides 
  forms 
  webapp 
  api 
```  
we select `sheets` and `Enter`


This will create a new Apps Sheet project in your Google Drive. with custom name project that we has defined.  
> We can save link that was generated both `googl apps script` and `google sheet`   in your README.md file   

- move `.clasp.json` from `src` directory to root
`In terminal ` 

```
mv src/.clasp.json .
```  

- create `Code.js` in `src` directory  

```bash
touch src/Code.js
```  

now we can push to upload to google apps script browser  
```bash
clasp push
```  

---  
---  
---   

## ✨ 2. Clone existing project to VSCode :  

<a href="#create-new-basic-directory-structure-in-vscode-use-npm">Create new Project</a>


```text
Project
├── ./src
├── LICENSE
├── package.json
└── README.md
```  

- find project Id in Apps Script browser project

https://github.com/user-attachments/assets/66da7190-1270-42fa-b3d6-0560401ca6d4

- clone app script project by ID: into `src` folder  

`In terminal`
```
clasp clone `<Id Project>` --rootDir src
```  

- move `.clasp.json` to root
In terminal  
```
mv src/.clasp.json .
```  
---  
---  
---  

### 🔨 push to Apps Script browser  
In terminal  
```
clasp push
```

### 🔨 pull to local machine  
In terminal  
```
clasp pull
```  

### 🔨 push and watch all changes  
In terminal
```
clasp push -w
```  

### 🔨 check files list that push to Apps Script browser  
In terminal  
```
clasp status
```
### 🔨 logout  
In terminal  
```
clasp logout
```

### Open the Apps Script browser on script.google.com:  
In terminal
```bash
clasp open
```  

### Open Web app  
In terminal  
```bash
clasp open --webapp
```  
> ### Find link that bound to Apps Script project  
- `clasp open` open Apps Script project in your browser
```bash
clasp open
```  

- Click on the "Overview" button in the left sidebar  
- Under "Project details", you'll see "Container" - this will have a link to your bound Google Sheet

### Run specific function  
In terminal  
```bash
clasp run 'myFunction'
```  

> 🎉 🎉 🎉 We can update from vscode editor and push it, refresh web page to see update on web browser


---  


## Resource  
- [Google Clasp :](https://github.com/google/clasp)  
- [Develop Google Apps Script Locally in VSCode using CLASP : On Youtube ](https://www.youtube.com/watch?v=lwxiEB-Mnys)
- [ครูอภิวัฒน์"สอนสร้างสื่อ : On Youtube"](https://www.youtube.com/@KruApiwat/playlists)  

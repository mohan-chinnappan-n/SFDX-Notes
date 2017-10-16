#### Create an App using SFDX

What is SF DX prject:

Local copy of your artifacts

What is artifact?

Group of releated code and customizations

Core assets to sync source and metadata with your scratch orgs


#### Creating a new project

```
$ sfdx force:project:create -n my-first-project
target dir = /Users/mchinnappan/sfdc/DX/Notes
   create my-first-project/sfdx-project.json
   create my-first-project/README.md
   create my-first-project/config/project-scratch-def.json
```

This command scaffolds this new project with all assets in the proper folder structure. 

Created folder structure:

```
$ tree
.
├── README.md
├── SFDX-setup.md
├── create-app.md
├── geolocation
│   ├── README.md
│   ├── config
│   │   └── project-scratch-def.json
│   ├── force-app
│   │   └── main
│   │       └── default
│   │           └── aura
│   └── sfdx-project.json
├── img
│   └── sfdx-active-scrath-orgs.png
└── my-first-project
    ├── README.md
    ├── config
    │   └── project-scratch-def.json
    ├── force-app <--- sourcecode for this project
    │   └── main
    │       └── default
    │           └── aura
    └── sfdx-project.json
    
```

```
$ cat my-first-project/sfdx-project.json 
{
  "packageDirectories": [
    {
      "path": "force-app",
      "default": true
    }
  ],
  "namespace": "",
  "sfdcLoginUrl": "https://login.salesforce.com",
  "sourceApiVersion": "41.0"
}
```


  

# FileTemplateModule
## Instruction how to create new domain sub-modules using this repository

### First of all you need to install plugin called ```Generate Module from Template```
> Android Studio -> Preferences -> Plugins -> Type Name ```Generate Module from Template```

### Download this files 
* https://github.com/PanVova/FileTemplateModule/blob/main/fileTemplateModule.zip
* https://github.com/PanVova/FileTemplateModule/blob/main/Domain%20module.json

### Installation:
 #### File with name fileTemplateModule need to be import 
> How to import settings: File -> Manage IDE Settings -> Import Settings -> Find file on PC
 #### File with name DomainModule.json 
> Tools -> Module Template Settings -> Tap "+" symbol -> Import from file -> Find file on PC


### Then you can add my existing template to create domain modules like ```impl, impl-rest, public```
<img width="693" alt="Screenshot 2022-05-17 at 14 53 49" src="https://user-images.githubusercontent.com/37262034/168806063-dafbc377-fb51-4def-ba68-29f068e5ef57.png">

### There you can change the package name, feature name and also don't forget to update feature name uppercase
<img width="722" alt="Screenshot 2022-05-17 at 14 54 11" src="https://user-images.githubusercontent.com/37262034/168806092-79de8339-d61e-4519-86d6-99a5d79e4464.png">

### As a result you will have a nice modules ```impl, impl-rest, public```

<img width="407" alt="Screenshot 2022-05-17 at 14 54 25" src="https://user-images.githubusercontent.com/37262034/168806108-f82428cd-d9ec-4b2b-a29b-e50bd162fccb.png">

### The last thing what you need to do is add all this 3 modules in ```settings.gradle``` 

```
include (
    ":someName:impl",
    ":someName:impl-rest",
    ":someName:public"
)
```
```someName``` - is the name of your feature

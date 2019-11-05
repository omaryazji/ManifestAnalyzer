# ManifestAnalyzer



## How to use

1. All installed applications on the device will be listed in the spinner.You have to select one from the list as shown in Screenshots 1&2
2. After selecting an app from the list. CLick Manifest Analyzer button as shown in Screenshots 3.
3. A new activity will be open to show the content of Manifest file of the selected app, s shown in Screenshots 4.

### Screenshot 1 & 2
![Screenshot_1572951087](https://user-images.githubusercontent.com/17234785/68202203-48245100-ffd4-11e9-9688-082996540b96.png)  ![Screenshot_1572951100](https://user-images.githubusercontent.com/17234785/68202204-48245100-ffd4-11e9-8e6d-dfb4ebb64e8a.png)
### Screenshot 3 & 4                                                                   
![Screenshot_1572951103](https://user-images.githubusercontent.com/17234785/68202206-48245100-ffd4-11e9-8a59-206722f2424b.png)      ![Screenshot_1572951106](https://user-images.githubusercontent.com/17234785/68202207-48bce780-ffd4-11e9-8272-689b8904fe5f.png)

## Technical Review
 ### MVC Architecture
  The project was built with 3 differnt layers and one interface for methods structure:  
  
    1. Model :  presents set of object classes that will be used during the interaction between other layers
    2. View  :  presents activites and user-interfaces and handle user interactions.
    3. Controller  : access, retrieve and manage application data
    4. Interfaces  : presents the structure of all methods used by object to interact with outside world

![image](https://user-images.githubusercontent.com/17234785/68207039-254b6a00-ffdf-11e9-8c15-3690bf89833b.png)


 ### Model
  * This layer contains **Application** object class with Name and Dir
  * Name: nmae of selected application
  * Dir: directory of the selected app apk file, this will be used to reach to Manifest file.
  * This object will be used to fill the spinner with installed applications list
  
```java
public class Application {
    public String Name;
    public String Dir;

    public Application(String name,String dir) {
        Name = name;
        Dir = dir;
    }

    public String getName() {
        return Name;
    }

    public void setName(String name) {
        Name = name;
    }

    @Override
    public String toString() {
        return Name;
    }
}
```

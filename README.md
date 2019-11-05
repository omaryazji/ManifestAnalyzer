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
  The project was built with 3 differnt layers :  
  
    1. Activites  layer - presents data to a screen and handle user interactions
    2. Interfaces layer - presents the structure of all methods used by object to interact with outside world
    3. Models  layer - presents set of object classes that will be used during the interaction between other layers
    4. Controller layer - access, retrieve and manage application data

![image](https://user-images.githubusercontent.com/17234785/68206840-c259d300-ffde-11e9-805d-c1efc8704be0.png)

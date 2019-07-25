

<h1><center>Global Functions</center></h1>

A common set of statements or operations can be defined globally as a function and it can be retrieved and used in any project. One global function shall be referred from another global function, But it should not be in circular reference. All the users have privilege to access global functions in calculated column, but admin and developer has an ability to create, edit and delete a global function.

> **Navigation : Settings → Global functions**

**1.**  Click on  **Add-Functions**  to create new function.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/d9712e86a6881444e961d60dfc6aab30bf665172/images/func1.png)

```
                                                      * My Custom function *
/*START*/ 
function myfunction(param1,param2,ParamN)
{
                                                      * Define function body *  
   return 0;

}
/*END*/
```

> **Note :**  You can add your code in function body only.

**For Instance**  Create a custom function for adding 2 parameters

```
                                                       * My Custom function *
/*START*/ 
function _Addition(param1,param2)
{
 var Addition = param1+param2;
  return Addition;
}
/*END*/
                                        
```
> **Note :**  To undo the changes done, click  **Undo**  icon. 
> To redo the changes made, click  **Redo**  icon.

**2.**  Click on  **Test**  Button to run the function.  

**3.**  Click on  **Save**  Button to save the function.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/2c15dfa03d8ed5eed5cdffdc1335c22ce759300c/images/global_functions.png)

## Ability to adopt JavaScript

This functions supports all the native java script supported functions and also refer other global functions using**bi.function_name**  ( param1, param2, paramN).

## Edit Function

**4.**  Enable edit key to  **Edit**  the function.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/22605db49d5ca324b621e568ed48fca35508adb0/images/New_version5/TD_Gobal_Functions_Image3.png)

## Delete Function

**5.**  Click delete button to  **Delete**  the function.

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAzNTQ5NjI1MiwtMTE2MTI5MDkzMiw3Mz
A5OTgxMTZdfQ==
-->


<h1><center>Global Functions</center></h1>

A common set of statements or operations can be defined globally as a function and it can be retrieved and used in any project. One global function shall be referred from another global function, But it should not be in circular reference. All the users have privilege to access global functions in calculated column, but admin and developer has an ability to create, edit and delete a global function.

> <b> Navigation : Settings → Global functions</b>

<b>1.</b>  Click on  <b>Add-Functions</b>  to create new function.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/5dbf9359490d4be550bbcf60addd600b5bde14ba/images/New_version5/TD_Gobal_Functions_Image4.png)
  <b><font color = "Black"> Image 1</font></b>
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

> <b>Note :</b>  You can add your code in function body only.

<b>For Instance</b>  Create a custom function for adding 2 parameters

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
> <b>Note :</b>  To undo the changes done, click  <b>Undo</b>  icon. 
> To <b>redo</b> the changes made, click  <b>Redo</b>  icon.

<b>2.</b>  Click on  <b>Test</b>  Button to run the function.  

<b>3.</b>  Click on  <b>Save</b>  Button to save the function.


![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/6ad2302fa77bfc83747a0f00223721b9ea23b471/images/New_version5/TD_Gobal_Functions_Image3.png)
  <b><font color = "Black"> Image 2</font></b>

## Ability to adopt JavaScript

This functions supports all the native java script supported functions and also refer other global functions using <b>bi.function_name</b> ( param1, param2,....paramN).

## Edit Function

**4.**  Enable edit key to  <b>Edit</b>  the function.

## Delete Function

<b>5.</b>  Click delete button to  <b>Delete</b>  the function.

<!--stackedit_data:
eyJoaXN0b3J5IjpbNDM5NzU1NjI3LC03OTc2NTA4MTIsMTUzOT
I4MTExMywzNTg2Nzg1NzAsLTMxMzc5MDA2MywyMTAyMTY0MDI3
LDE0NzI5NTg5NjYsLTI2MTk2MTk1MiwxMjE5NTU5Mzc0LC0xMT
YxMjkwOTMyLDczMDk5ODExNl19
-->
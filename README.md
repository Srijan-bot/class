# filehandling
<br>

## What is data file?
<br>
<p>The files that store data pretaining to a specfic applicatoion for later use.</p>
<br>

## Type of data files =>

1. **Text File**
   1. _RTF(Regular text files)_
   1. _DTF(Delimited text files)_
    * > TSV files(tab seprated value)<br>
    * > CSV files(comma seprated value)
<br>

2.**Binary Files**

**_ lets see the code itself :grin: _**
<br>

[Sample file](https://github.com/Srijan-bot/filehandling/blob/main/sample.txt)
<br>

[Code File](https://github.com/Srijan-bot/filehandling/blob/main/one.py)
<br>
<!-- 1. Item 2 -->


<br>

 **Opening & Closing of file**

 > *syntax:* <file_objectname>=open(<file_name>)

```
f=open("sample.txt","r")
f.close()
```
> Type of function for opening a file.

Symbol | Symbol(Binary) | Name | Function
------------ | ------------ | ------------- | -------------
`r` | `rb` | Read mode | allow file to read-only.
`w` | `wb` | Write mode | allow file to edit in overwrite.
`a` | `ab` | Append mode | allow file to edit **without** overwriting it.

# Read mode (r)

> note! read is **Default** mode means f=open("sample.txt","r") & f=open("sample.txt) are exatly same!.

```
f=open("sample.txt","r")
```
:point_up_2: This will open sample file in `f` object.

```
f=open("1.txt","r")
```
:point_up_2: This will genrate error shown as follow:
> FileNotFoundError: [Errno 2] No such file or directory: '1.txt'

<hr>

### reading file

```
f=open("sample.txt","r")
read=f.read()
print(read)
f.close()

```
output will be: :point_down:

`This gritty portrayal of art through adversity picks up where the author left us in Train of
Thought; Poems from the Red Line. The book begins in Kendall Square, the home of M.I.T; moves on
 to Central Square, the land of the Out of the Blue Gallery, The Middle East, and once T.T the
Bears; on to Harvard with the Hahvad Punk kids; and exits at the home of famed Johnny Dâ€™s, Davis
 Square. Join a poet with time to kill on the MBTA, with his worst enemy, his mind, and his best
  friend, the pen.`

#### Raw vs. PureString

Raw String:
 The string is used when there is so special meaning attach to any charcter. It uses prefix `r` before the path.
 > syntax:

 ```

 f=open(r"./class/sample.txt")

 ```  
 Path String:
 This is the orignal way of showing the path in python.
 > syntax:
 ```
 f=open(".//class//sample.txt")
 ```
 
 <hr>

 ## **Working with files**

 reading text files :-

 Method | Syntax | Description 
------------ | ------------ | ------------- 
`read()` | ``` f.read([n]) ``` | Read mode 
`w` | `wb` | Write mode 
`a` | `ab` | Append mode 



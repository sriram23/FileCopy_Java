# FileCopy_Java
- The code will copy a directory in a particular path and will paste in a destination.
- For this we need to import *external jar* called **commons-io**. We can get the jars [here](https://commons.apache.org/proper/commons-io/download_io.cgi).

## How to import external Jars in Eclipse IDE:
- Right click the project -> Build Path -> Add External Archieves
![Screen shot of Adding External Jars](https://github.com/sriram23/FileCopy_Java/blob/master/jar.png)

- Select all the *Jar* files and click open. The jar files will be imported.

## Source Code
```
import java.io.*;
import org.apache.commons.io.FileUtils;
public class FileCopy {
	public static void main(String args[]){
		File source = new File("C:\\Users\\cslab.admin-PC\\Desktop\\Hello World");
		File destination = new File("C:\\Users\\cslab.admin-PC\\Desktop\\HelloCopy");
		try{
			FileUtils.copyDirectory(source, destination);
		}catch(IOException e){
			e.printStackTrace();
		}
	}
}
```

## Output:
![Screen Shot of Output](https://github.com/sriram23/FileCopy_Java/blob/master/Capture.JPG)

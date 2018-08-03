# Jenkins-test

--> To run a selenium project from command prompt. Do the followng steps-
1. My project location is this - C:\Users\A622893\Desktop\Jenkins-test\Selenium
2. Create a lib(anyname) folder inside selenium(project) and place all jar file(including chromediver).
3. Now open the cmd prompt and set the class path by the following cmd-
   cmd- set classpath=C:\Users\A622893\Desktop\Jenkins-test\Selenium\bin;C:\Users\A622893\Desktop\Jenkins-test\Selenium\lib*;
4. Now type the cmd toexecute the selenium testng project from cmd prompt-
   cmd- java org.testng.TestNG testng.xml
   
--> To run a selenium project from command prompt using batch file( perform all above steps first then do this step). Do the followng steps-
1. Go to the poject location.i.e - C:\Users\A622893\Desktop\Jenkins-test\Selenium
2. Create a test file and type the following cmd inside it.
   cmd- java -cp bin;lib/* org.testng.TestNG
3. Now do the save as and save file using double quotes "run.bat". If you see, file type will be windows batch file.

--> To run a selenium project from Jenkins ( perform all above steps first then do this step). Do the followng steps-
1. Install jenkins, set creds, create a new project.
2. Configure it and mention following details-
   General>advance section> ticket the checkbox of "Use custom workspace". and mention the directory path -> C:\Users\A622893\Desktop\Jenkins-test\Selenium
   Build-> Execute Windows batch command. Cmd- run.bat
3. Now save the settings. and run the project.
   Thats it.
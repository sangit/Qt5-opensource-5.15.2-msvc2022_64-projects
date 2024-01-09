# Qt5-opensource-5.15.2-msvc2022_x64-projects #
## Qt5 x64 Application Development in VS 2022 ##

These are free tools for qt-5.15.2-msvc2019_64 downloaded by qt-unified-windows-x64-4.6.1-online.exe.

<br />

## **First Technique(direct copying dlls if Qt5 isnot in path/unzipped):**
Copy the appropriate folder's all files into correct build folder where is your exe file.

If some extra plugins are required copy them from Qt5's plugins\platform folder.

For other required qt5 dlls copy them from Qt5's bin folder.

<br />

## **Second Technique(If Qt5 is in path/installed):** ##

This is mentioned in https://wiki.qt.io/Deploy_an_Application_on_Windows

After adding required libs and include, build the project and test by running.

Make a folder, for example named deployment and copy the exe file.

Open Start menu->Visual Studio 2022->x64 Native Tools for VS 2022.

Run the command: Drive_To_Qt5\Qt5WhereEverFolder\bin\windeployqt.exe  Drive_To_Exe:\ExeWhereEverFolder\deployment\project.exe

For example C:\Qt5\bin\windeployqt.exe E:\test_project\deployment\test.exe

Automatically all dependencies will be copied into the folder.

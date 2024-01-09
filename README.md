# Qt5-opensource-5.15.2-msvc2022_64-projects
Qt5 Application Development in VS 2022


These are free tools for qt-5.15.2-msvc2019_64 downloaded by qt-unified-windows-x64-4.6.1-online.exe.




First technique(direct copying dlls if Qt5 isnot in path/unzipped):

Copy the appropriate folder's all files into correct build folder where is your exe file.

If some extra plugins are required copy them from Qt5's plugins\platform folder.

For other required qt5 dlls copy them from Qt5's bin folder.




Second technique(If Qt5 is in path/installed):

This is mentioned in https://wiki.qt.io/Deploy_an_Application_on_Windows

After adding required libs and include, build the project and test by running.

Make a folder, for example deployment and copy the exe file.

Open Start menu->Visual Studio 2022->x64 Native Tools for VS 2022.

Run the command: Drive_to_qt5\qt5_where_ever_folder\bin\windeployqt.exe  Drive_to_exe:\exe_where_ever_folder\deployment\project.exe

For example C:\Qt5\bin\windeployqt.exe E:\test_project\deployment.\test.exe

Automatically all dependencies will be copied into the folder.

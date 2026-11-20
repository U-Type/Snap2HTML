# Snap2HTML
This application takes a "snapshot" of the folder structure on your harddrive and saves it as an HTML file. What's unique about Snap2HTML is that the HTML file uses modern techniques to make it feel like a "real" application, displaying a treeview with folders that you can navigate to  view the files contained within. There is also a built in file search and ability to export data as plain text, csv or json. Still, everything is  contained in a single HTML file that you can easily store or distribute.

Homepage with examples and binary downloads: http://www.rlvision.com/snap2html

## Build on Windows 11

1. Install [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/) with the **.NET desktop development** workload. Under **Individual components**, select the **.NET Framework 4.8 targeting pack** and **.NET Framework 4.8 SDK**. For an existing installation, open Visual Studio Installer and select **Modify**.
2. Open `Snap2HTML.sln` in Visual Studio. If you downloaded the source as a ZIP, right-click the ZIP, choose **Properties**, select **Unblock** if shown, and then extract it before opening the solution.
3. In the toolbar, choose **Release** and **Any CPU**. Select **Build > Build Solution** (`Ctrl+Shift+B`). Press `Ctrl+F5` to run the app.
4. The executable is `Snap2HTML\bin\Release\Snap2HTML.exe`. To run it elsewhere, copy the whole Release folder so that `template.html` stays beside the executable.

For subsequent command-line builds, open **Developer Command Prompt for Visual Studio**, change to the folder containing `Snap2HTML.sln`, and run:

```bat
msbuild Snap2HTML.sln /p:Configuration=Release /p:Platform="Any CPU"
```

## Screenshots

WinForms application for generating the direcotry listings:

<img src="http://www.rlvision.com/snap2html/screenshot.png">

The finished HTML app:

<img src="http://www.rlvision.com/snap2html/example.png">

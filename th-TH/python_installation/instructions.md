> สำหรับผู้อ่านทางบ้าน: บทนี้ครอบคลุมวิดีโอในส่วนของ [การติดตั้ง Python และ Code Editer](https://www.youtube.com/watch?v=pVTaqzKZCdA)
> 
> ในส่วนของบทนี้ อ้างอิงมาจากบทเรียนของ Geek Girls Carrots (https://github.com/ggcarrots/django-carrots)

Django ถูกเขียนโดยภาษา Python เพราะฉะนั้นเราจึงต้องใช้ Python ในการทำอะไรต่างๆใน Django งั้นเรามาเริ่มต้นด้วยการติดตั้ง Python กันเถอะ คุณต้องติดตั้ง Python เวอร์ชั่น 3.6 ถ้าหากคุณมีเวอร์ชั่นก่อนหน้านี้ คุณควรที่จะอัพเกรดมันก่อนนะ

<!--sec data-title="Install Python: Windows" data-id="python_windows" data-collapse=true ces-->

First check whether your computer is running a 32-bit version or a 64-bit version of Windows, on the "System type" line of the System Info page. To reach this page, try one of these methods:

* Press the Windows key and Pause/Break key at the same time
* Open your Control Panel from the Windows menu, then navigate to System & Security, then System
* Press the Windows button, then navigate to Settings > System > About

You can download Python for Windows from the website https://www.python.org/downloads/windows/. Click on the "Latest Python 3 Release - Python x.x.x" link. If your computer is running a **64-bit** version of Windows, download the **Windows x86-64 executable installer**. Otherwise, download the **Windows x86 executable installer**. After downloading the installer, you should run it (double-click on it) and follow the instructions there.

One thing to watch out for: During the installation, you will notice a window marked "Setup". Make sure you tick the "Add Python 3.6 to PATH" checkbox and click on "Install Now", as shown here:

![Don't forget to add Python to the Path](../python_installation/images/python-installation-options.png)

When the installation completes, you may see a dialog box with a link you can follow to learn more about Python or about the version you installed. Close or cancel that dialog -- you'll be learning more in this tutorial!

In upcoming steps, you'll be using the Windows Command Line (which we'll also tell you about). For now, if you need to type in some commands, go to Start menu and enter "Command Prompt" into the search field there. (On older versions of Windows, you can start the Command Line with Start menu → Windows System → Command Prompt.) You can also hold in the Windows key and press the "R"-key until the "Run" window pops up. To open the Command Line, type "cmd" and press enter in the "Run" window.

![Type "cmd" in the "Run" window](../python_installation/images/windows-plus-r.png)

Note: if you are using an older version of Windows (7, Vista, or any older version) and the Python 3.6.x installer fails with an error, you can try either:

1. ติดตั้ง Windows Updates ทั้งหมด และลองติดตั้ง Python 3.6 อีกครั้ง; หรือ
2. ติดตั้ง [Python รุ่นเก่า](https://www.python.org/downloads/windows/) เช่น e.g., [3.4.6](https://www.python.org/downloads/release/python-346/)

If you install an older version of Python, the installation screen may look a bit different than shown above. Make sure you scroll down to see "Add python.exe to Path", then click the button on the left and pick "Will be installed on local hard drive":

![Add Python to the Path, older versions](../python_installation/images/add_python_to_windows_path.png)

<!--endsec-->

<!--sec data-title="Install Python: OS X" data-id="python_OSX"
data-collapse=true ces-->

> **หมายเหตุ** ก่อนที่คุณจะติดตั้ง Python บนระบบปฏิบัติการ OS X คุณควรตรวจสอบให้แน่ใจว่าการตั้งค่า Mac ของคุณนั้นอนุญาตให้ติดตั้งแพคเก็จที่ไม่ได้มาจาก App Store ได้ ให้ไปที่ System Preferences (มันอยู่ในโฟลเดอร์ Applications) คลิก "Security & Privacy," หลังจากนั้นให้คลิกที่แท็บ "General" ถ้าหาก "Allow apps downloaded from:" ถูกตั้งค่าให้อยู่ใน "Mac App Store," ให้เปลี่ยนเป็น "Mac App Store and identified developers."

You need to go to the website https://www.python.org/downloads/release/python-361/ and download the Python installer:

* Download the *Mac OS X 64-bit/32-bit installer* file,
* Double click *python-3.6.1-macosx10.6.pkg* to run the installer.

<!--endsec-->

<!--sec data-title="Install Python: Linux" data-id="python_linux"
data-collapse=true ces-->

It is very likely that you already have Python installed out of the box. To check if you have it installed (and which version it is), open a console and type the following command:

{% filename %}command-line{% endfilename %}

    $ python3 --version
    Python 3.6.1
    

If you have a different 'micro version' of Python installed, e.g. 3.6.0, then you don't have to upgrade. If you don't have Python installed, or if you want a different version, you can install it as follows:

<!--endsec-->

<!--sec data-title="Install Python: Debian or Ubuntu" data-id="python_debian" data-collapse=true ces-->

Type this command into your console:

{% filename %}command-line{% endfilename %}

    $ sudo apt install python3.6
    

<!--endsec-->

<!--sec data-title="Install Python: Fedora" data-id="python_fedora"
data-collapse=true ces-->

Use this command in your console:

{% filename %}command-line{% endfilename %}

    $ sudo dnf install python3
    

If you're on older Fedora versions you might get an error that the command `dnf` is not found. In that case, you need to use `yum` instead.

<!--endsec-->

<!--sec data-title="Install Python: openSUSE" data-id="python_openSUSE"
data-collapse=true ces-->

Use this command in your console:

{% filename %}command-line{% endfilename %}

    $ sudo zypper install python3
    

<!--endsec-->

Verify the installation was successful by opening a command prompt and running the `python3` command:

{% filename %}command-line{% endfilename %}

    $ python3 --version
    Python 3.6.1
    

**NOTE:** If you're on Windows and you get an error message that `python3` wasn't found, try using `python` (without the `3`) and check if it still might be a version of Python 3.6.

* * *

If you have any doubts, or if something went wrong and you have no idea what to do next, please ask your coach! Sometimes things don't go smoothly and it's better to ask for help from someone with more experience.
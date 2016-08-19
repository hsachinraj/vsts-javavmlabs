## Working with Git


Adding existing code to Git
---------------------------

In this exercise, you are going to learn how to put some existing code
into your Team Project. This exercise assumes you have completed
Exercise 1, and have created a Team Project that uses Git for version
control and have completed Exercise 2 where you’ve defined some work
items. This exercise uses a team project named **jdev**, though your
team project name may differ.

1.  Open Eclipse from the Launcher by clicking on the **Eclipse** icon.

    <img src="./images/git/image2.png" width="594" height="126" />

2.  When the **Workspace Launcher** appears, you can accept the default
    folder or select another one. This is where Eclipse will store
    your projects. You can select the **Use this as the default and do
    not ask again** option if you want Eclipse to remember the folder
    and do not prompt every time on startup.

    Select **OK** when you are done.

    <img src="./images/git/image3.png" width="490" height="248" />

3.  Open the **Team Foundation Server Explorer** perspective. To open
    the Team Foundation Server Exploring perspective:

    1.  On the **Window** menu, point to **Open Perspective**, and click
        **Other**.

    2.  In the **Open Perspective** dialog box, click **Team Foundation
        Server Exploring**, and then click **OK**.

        <img src="./images/git/image4.png" width="624" height="278" />

<pre><b>Note:</b> A perspective defines the initial set and layout of views in the Workbench window. 
You can create new or customize existing perspectives. If you want to know more, you might find this
[tutorial](http://www.tutorialspoint.com/eclipse/eclipse_perspectives.htm) helpful </pre>

1.  If necessary, click the Home icon. Click the **Connect to Team
    > Foundation Server** link.

    <img src="./images/git/image5.png" width="182" height="239" />

1.  In the **Add Existing Team Project** dialog, click the
    **Servers** button.

    <img src="./images/git/image6.png" width="439" height="224" />

1.  In the **Add/Remove Team Foundation Server** dialog, click the
    **Add** button on the right. Enter the name of your Visual Studio
    Team Services account plus **.visualstudio.com**. For example, if
    your account name is *javadev*, you would enter
    *javadev.visualstudio.com* (without any http or https). Once
    you’ve entered your account name, click **OK**.

    <img src="./images/git/image7.png" width="284" height="184" />

2.  In the login dialog that appears, enter your alternate username and
    password and click **OK**.

    <img src="./images/git/image8.png" width="414" height="209" />

3.  Choose the **Team Project** (jdev) and select **Finish**

    <img src="./images/git/image9.png" width="434" height="190" />

4.  Eclipse will open a Secure Storage dialog. Enter a password and
    confirm it in the dialog and click **OK**.

<pre>Eclipse stores the connection information in an encrypted form in a
storage file that is stored with a predefined password. Make sure you
can remember this password. Eclipse will offer to allow you to save
password hints for password recovery. Click Yes or No depending upon
your needs.</pre>

<img src="./images/git/image10.png" width="364" height="276" />

1.  Now click **Close** in the **Add/Remove Team Foundation Server** dialog.

2.  In the **Add Existing Team Project** dialog, select the **Default
    Collection** and then select your **jdev** Team Project from the
    list and click **Finish**.

3.  Upon successful connection, you will see Team Explorer window
    showing source control, work items, build and settings menu.

    <img src="./images/git/image11.png" width="235" height="288" />

Cloning Git Repository
----------------------

1.  In the **Team Explorer** window, click the **Git
    Repositories** tile.

2.  In the list of repositories, select the bottom **jdev** node.

    <img src="./images/git/image12.png" width="346" height="143" />

1.  Right-click on the **jdev** node and select **Import Repository**.

    <img src="./images/git/image13.png" width="225" height="138" />

In the dialog that opens click **Next**.

    <img src="./images/git/image14.png" width="304" height="273" />

1.  In the Import Projects from Team Foundation Server dialog,

    -   Change the **Destination** to use the **Location** option and
        select user’s home folder.

    -   In the **Authentication** group, provide your alternate
        credentials you created in Exercise 1, step 22. Feel free to
        place a check next to **Save password**. Click **Next**
        when ready.

        <img src="./images/git/image15.png" width="339" height="433" />

2.  On the **Clone Summary** page, click **Next**.

    <img src="./images/git/image16.png" width="377" height="124" />

1.  Enter your alternate credentials when prompted and click **OK**.

2.  On the **Select Project Import Wizard** page, click **Next**.

    <img src="./images/git/image17.png" width="257" height="281" />

3.  You don’t have any existing Eclipse projects so just click
    **Finish**.

    <img src="./images/git/image18.png" width="271" height="333" />

    At this point you’re going to add the sample code already installed
    on the VM and copy it into your local repo where you’ll then commit
    and then push up to VS Team Services.

4.  Open File Manager and navigate to the **/home/vmadmin** folder. Copy
    all of the **myshuttle** folders – myshuttle, myshuttle.extras,
    myshuttle.UITest, myshuttle.ARM

    <img src="./images/git/image19.png" width="452" height="355" />

5.  Copy or move them to your home folder **(/home/&lt;user name&gt;**)

    <img src="./images/git/image20.png" width="445" height="352" />

6.  Open myshuttle folder. Select all the files in the folder. Right
    click and select **Copy**

    <img src="./images/git/image21.png" width="403" height="251" />

7.  Go to the **jdev** folder and paste the copied files

    <img src="./images/git/image22.png" width="440" height="283" />

8.  Return back to Eclipse.

9.  Activate the **Java EE** Perspective by click its button in the
    upper right corner, to the left the **Team Foundation Server
    Explorer** button.

    <img src="./images/git/image23.png" width="523" height="190" />

1.  Right-click in the **Project Explorer** and select **Import |
    Import**.

    <img src="./images/git/image24.png" width="320" height="292" />

1.  In the **Import** dialog, select **Projects from Git** from under
    the **Git** node and select **Next.**

    <img src="./images/git/image25.png" width="351" height="144" />

1.  Select **Existing local repository** and click **Next.**

    <img src="./images/git/image26.png" width="350" height="218" />

1.  Select **jdev** from the list and click **Next**.

    <img src="./images/git/image27.png" width="397" height="249" />

2.  Select import as general project.

    <img src="./images/git/image28.png" width="379" height="284" />

1.  Click **Next** and then click **Finish** on the final page.

2.  You should be able to see the project now in the **Project
    Explorer** window.

    <img src="./images/git/image29.png" width="227" height="211" />

Configuring User Name and Email for Git
---------------------------------------

Now before you can commit artifacts to the local repo and the push to VS
Team Services, you need to configure your user name and e-mail address
for Git in Eclipse.

1.  Select **Window | Preferences**. Under the **Team** node, select
    **Configuration** under the **Git** node.

2.  On the **Configuration** page, click **Add Entry**. In the resulting
    > dialog, enter **user.name** in the **Key** field and in the
    > **Value** field, enter your *display name* and click **OK**.

3.  Click **Add Entry** again to make another entry. Enter
    **user.email** in the **Key** field and in the **Value** field,
    enter your *e-mail address* and click **OK**.

    <img src="./images/git/image30.png" width="467" height="346" />

4.  Click **OK** to save your preferences.

<pre>You’re now ready to take your local changes and commit them locally and then push them up to 
your remote repository in Visual Studio Team Services.</pre>

Committing changes to Git
-------------------------

1.  In the **Project Explorer**, right click on the root node and select
    **Team | Commit**. You can alternatively press **CTRL+\#** key

    <img src="./images/git/image31.png" width="425" height="340" />

1.  In the **Commit Changes** dialog, enter a commit message like **Add
    existing files** followed by \#123 where 123 is the Work Item ID
    for one of your PBIs. If you don’t remember the Work Item ID,
    switch over to your open web browser and take a look at the
    Backlog or Task Board.

2.  In the Files section click the
    <img src="./images/git/image32.png" width="18" height="23" /> button to
    select all the files.

3.  Now click **Commit and Push**.

    <img src="./images/git/image33.png" width="282" height="294" />

1.  Once the process is complete, click **OK** to close the **Push
    Results** dialog.

    Let’s see what you can see using the Visual Studio Team Services
    website for the project. Switch back to your web browser.

2.  Click the **Code** link at the top. You can see the code you just
    pushed into the repository.

> <img src="./images/git/image34.png" width="311" height="269" />

1.  Click the **History** tab to see the information on the push you
    just performed.

2.  Click the **Explorer** link, and then expand the **src** folder
    under the **jdev** root until you find the **DataAccess.java**
    file (jdev/src/main/java/com/microsoft/example). Select that file.

    <img src="./images/git/image35.png" width="468" height="273" />

1.  You can easily browse the file. As you can see Visual Studio Team
    Services understands that this is a particular type of file and
    applies syntax formatting.

2.  Select the root **jdev** node.

3.  Leave your browser open and on the current page. Continue to the
    next exercise where you’ll configure a Team Build.



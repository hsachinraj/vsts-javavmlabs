
# Exercise 11: Monitoring your application with Application Insights

Application Insights is an extensible analytics service that monitors your live application. It helps you detect and diagnose performance issues, and understand what users actually do with your app. It&#39;s designed for developers, to help you continuously improve the performance and usability of your app. You can find more about Application Insights at [https://azure.microsoft.com/en-us/documentation/articles/app-insights-overview/](https://azure.microsoft.com/en-us/documentation/articles/app-insights-overview/)

In this exercise, you will learn how to configure Application Insights to monitor your web application that you have just released.

## Creating a new Application Insights resource:

1. From your VM, start Firefox and login to your [Azure portal](https://portal.azure.com/)

2. Create a new Application Insights  resource  
![](https://github.com/hsachinraj/vsts-javavmlabs/blob/master/HoLs/images/AIonAzurePortal.png?raw=true)
 
3. Select the **Create** button

4. Enter a name for the Application Insights resource. Let&#39;s say we name this **myshuttle-vstsjltomcat**. Select **Java web application** for **Application Type**.
![](https://github.com/hsachinraj/vsts-javavmlabs/blob/master/HoLs/images/AI-2.png?raw=true)
5. Select the **Create** button for Azure to start provisioning the resource. This should be ready in a minute or two. Once it is provisioned, open it and select the **Settings and Diagnostics** link and choose **Properties**. Note the **Instrumentation Key** in the properties window. We will need this later
![](https://github.com/hsachinraj/vsts-javavmlabs/blob/master/HoLs/images/AI-3.png?raw=true)


## Downloading the AI Binaries
6. You will need the Application Insights binaries to be copied to your machine. Open a new tab in your browser and navigate to   [http://aka.ms/ailab](http://aka.ms/ailab)

7. Download the **Application Insights – Java SDK.zip** fileto your local machine. When prompted to save, choose **Open with Archive Manager.** You can ignore the other two files.
![](https://github.com/hsachinraj/vsts-javavmlabs/blob/master/HoLs/images/AI-4.png?raw=true)

8. Select **Extract** and in the location dialog, select **Create Folder**  and create a folder with the name **AI SDK**
![](https://github.com/hsachinraj/vsts-javavmlabs/blob/master/HoLs/images/AI-5.png?raw=true)

9. Select **Extract** to complete extracting. Once the Extraction is completed, select **Show the Files** option or just simply quit and use the **File Manager** to go to your home folder.

10. Open the **AI SDK** folder and you will see a number of JAR files downloaded. Right-click the **Application Insights.xml** file and select **Open with – Open with &quot;gedit&quot;** option




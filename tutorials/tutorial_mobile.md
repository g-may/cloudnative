---
copyright:
  years: 2017, 2018
lastupdated: "2018-01-19"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# Mobile Basic Starter
{: #tutorial}

The following end-to-end tutorial walks you through the steps to create a mobile project from a Mobile Basic Starter. This guide includes installing prerequisite tools, and the steps to run the project in Xcode and Android Studio.


## Installing developer tools
{: #dev_tools}

Ensure that you install the [IBM Cloud Developer Tools](../idt/index.html#add-cli){: new_window}.


## Choose how to create your project
{: #choose_how}

You can create a project by using one of the following methods, based on your preference:
- Web-based [{{site.data.keyword.dev_console}}](#create-devex)
- Local command-driven [{{site.data.keyword.dev_cli_notm}}](#create-cli)


## Creating a project by using the {{site.data.keyword.dev_console}}
{: #create-devex}

1. Create a {{site.data.keyword.dev_console}} project in {{site.data.keyword.Bluemix}}.

    1. From the [**Starter Kits** ![External link icon](../icons/launch-glyph.svg "External link icon")](https://console.ng.bluemix.net/developer/appservice/starter-kits/) page in the {{site.data.keyword.dev_console}}, select a Starter Kit based on your chosen capabilities. For example, for a Watson Language application, go to **Watson Language** and click **Select Starter Kit**.

    2. Enter your project name. For this tutorial, use `WatsonProject`.   

    3. Select your language platform. For this tutorial, use `Swift`.

    4. Click **Create Project**.

## Optional: Add services
{: #add-services}

1. Select your project in the **Projects** page. 

2. Click **Add Service**.

3. Select the kind of service you want. For this tutorial, select **Security** > **Next** > **App ID** > **Next**.

4. Enter your service name and click **Create**.

5. For more information about configuring Authentication, see [Configuring identity providers ![External link icon](../icons/launch-glyph.svg "External link icon")](/docs/services/appid/identity-providers.html){: new_window}.

6. For more information about configuring Analytics, see [Getting started with {{site.data.keyword.mobileanalytics_short}} ![External link icon](../icons/launch-glyph.svg "External link icon")](/docs/services/mobileanalytics/index.html){: new_window}.

7. For more information about configuring {{site.data.keyword.cloudant_short_notm}}, see [Getting started with {{site.data.keyword.cloudant_short_notm}} ![External link icon](../icons/launch-glyph.svg "External link icon")](/docs/services/Cloudant/index.html){: new_window}.

8. For more information about configuring {{site.data.keyword.objectstorageshort}}, see [Getting started with {{site.data.keyword.objectstorageshort}} ![External link icon](../icons/launch-glyph.svg "External link icon")](/docs/services/ObjectStorage/index.html){: new_window}.

9. For more information about adding the Push Notifications capability, see:

    1. For iOS, [configure Apple Push Notification Service ![External link icon](../icons/launch-glyph.svg "External link icon")](/docs/services/mobilepush/t_push_provider_ios.html){: new_window}.

    2. For Android, [configure Firebase Cloud Messaging ![External link icon](../icons/launch-glyph.svg "External link icon")](/docs/services/mobilepush/t_push_provider_android.html){: new_window}.


## Generate your project code
{: #generate-code}

1. Select your project in the **Projects** page. 

2. Click **Download Code** to download your project archive.


## Begin working on your app
{: #code}

Begin working with your downloaded project:

1. Expand the archived file.

2. Navigate to the new project directory.

3. Use the {{site.data.keyword.dev_cli_notm}} to proceed.


## Creating a project by using the {{site.data.keyword.dev_cli_notm}}
{: #create-cli}

1. Ensure that you install the [{{site.data.keyword.dev_cli_short}}](../idt/index.html).

2. In your Terminal prompt, navigate to a local directory of your choice and run the following command.

	```
	bx dev create
	```
	{: codeblock}
	
3. Provide the following values when prompted:

	* Select a project type of "Mobile Client", option 2
	* Select implementation language to be "iOS Swift", option 3
	* Select starter kit of "Mobile App: Basic", option 1
	* Enter a name for your project: `MobileBasicProject`

    Note: Actual selection numbers may change with tooling enhancements.

4. If you want to add services to your project, type `y` at the question prompt and answer the remaining questions.

5. When your `MobileBasicProject` is successfully created and saved, navigate to the `MobileBasicProject/MobileBasicProject-Swift` folder.


## Running your Swift project in Xcode
{: #run_swift}

1. Open the `README.md` file in a Markdown viewer to review the steps to configure your project.

2. Open your Terminal and navigate to your project folder, and execute the following commands:
    1. Run `pod setup` if you need to set up your CocoaPods repository.
    2. Run `pod update` if you need to update you update your existing pods.
    3. Run `pod install` to install the pods for your project.

3. Open your `<projectname>.xcworkspace` Xcode workspace.

4. Run your app.


## Running your Cordova project in Xcode
{: #run_cordova_xcode}

If you opted to use Cordova as tyour implementation language, then follow these instructions.

1. Open the `README.md` file in a Markdown viewer to configure your project.

2. Open your `platforms/ios` project in Xcode.

3. Run your app.


## Running your Cordova project in Android Studio
{: #run_cordova_studio}

Use this section if you chose to use Cordova as you mobile app's platform.

1. Extract the `BasicProject-Cordova.zip` file.

2. Open the `README.md` file in a Markdown viewer to configure your project.

3. Open your `platforms/android` project in Android Studio.

4. Run your app.


## Running your Android project in Android Studio
{: #run_android}

Use this section if you chose to use Android as you mobile app's platform.

1. Open the `README.md` file in a Markdown viewer to configure your project.

2. Open your `BasicProject-Android` project in Android Studio.

3. Run your app.
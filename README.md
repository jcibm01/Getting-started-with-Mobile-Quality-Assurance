Getting-started-with-Mobile-Quality-Assurance
=============================================

Getting started with Mobile Quality Assurance

Tomado de https://www.ng.bluemix.net/docs/#services/MobileQualityAssurance/index.html#mqaov001

Use IBM® Mobile Quality Assurance for Bluemix™ to discover and set up mobile quality services for your apps. You can view high-level quality metrics for your mobile apps to get a quick understanding of the issues for apps that you are working on. These metrics include information for crashes, bugs, user feedback, and user sentiment. By viewing this information for your apps, you can determine whether to investigate specific issues further. For example, if the crash rate for an app spikes, you can click the crash rate to view more detailed information on crash reports for that app.

To set up mobile quality services for apps, complete the following tasks:

    Create a Mobile Quality Assurance service instance:
        From the Bluemix catalog, scroll to either the Mobile or DevOps section, select MobileQualityAssurance, and then click CREATE SERVICE.
        Optional: Specify the existing app that you want to add the Mobile Quality Assurance service to.
        Click CREATE. The new service is displayed in the Services section.
    Before you can begin to use this new Mobile Quality Assurance service, you must first add the service to a Mobile Quality Assurance app:
        In the Services section, click the Mobile Quality Assurance service.
        In the tile that opens, click New MQA App.
        Specify a name for the new Mobile Quality Assurance app.
    After you add the Mobile Quality Assurance service instance to the Mobile Quality Assurance app, you must prepare the app for reporting:
        Select a platform for your new app (such as iOS). Click Add Platforms, select the platform and then click Submit.
        Tip: An app can have multiple platforms. To select more than one platform for your app, repeat this step and choose each additional platform that you want to select (such as Android).
        Download and install the libraries for the selected platform to instrument your new app to start collecting data:
        Library 	Description
        Pre-production 	Install the pre-production libraries so that internal testers can provide detailed information about bugs and crashes that occur with your app.
            In the Pre-production section, click the following links:
                pre-production SDK to download the pre-production SDK for the selected platform.
                MQA App key to obtain your Mobile Quality Assurance application key. In the Application Details page, locate your application key.
                Screen capture of Application Key in the Mobile Quality Assurance application.
            Use the downloaded SDK and app key to instrument your app:
                Android SDK
                iOS SDK
                Worklight® SDK

        After the first session is recorded, details for the app are displayed.
        Production 	Install the production libraries so that users can provide detailed information about your app. If your app is in production, Mobile Quality Assurance facilitates getting feedback from users right within the app.
            In the Production section, click the following links:
                production SDK to download the production SDK for the selected platform.
                MQA App key to obtain your Mobile Quality Assurance application key. In the Application Details page, locate your application key.
            Use the downloaded SDK and app key to instrument your app:
                Android SDK
                iOS SDK
                Worklight SDK

        After the first session is recorded, details for the app are displayed.
    To view the overall health of the app, set the user insights for that app:
        In the Get insights from user reviews section, click the link to configure sentiment analysis.
        Tip: This feature works only for apps that exist in the App stores.
        In the Application Details page, configure sentiment analysis and save your changes.
        View the overall score for the selected app within the Mobile Quality Assurance service instance:
        Screen capture of overall score for a selected app.

Getting started with viewing quality metrics for apps
You can view high-level quality metrics for your mobile apps to get a quick understanding of the issues for apps that you are working on. These metrics include pre-production data for crashes and bugs and production data for crashes, feedback, and sentiment.

By viewing this information for your apps, you can determine whether to investigate specific issues further. For example, if the crash rate for an app spikes, you can click the crash rate to view more detailed information on crash reports for that app.
To view more detailed quality information for an app, click any of the following options:
Screen capture of quality metrics for an app
Option 	Description
Sessions 	Review information about crashes, bugs, and the state of the device during the session.
Crashes 	Review information about what happened to cause crashes.
Bugs 	Review information reported by users such as bug reports, screen captures, and device details.
Feedback 	Review user feedback responses to see who wrote the feedback, and when.
Sentiment Score 	Review the user sentiment score over time and versions to monitor, measure, and improve app quality.
Registered Devices 	Review the list of devices that are used during a testing session and information about these devices.
Mobile Quality Assurance overview

IBM Mobile Quality Assurance for Bluemix equips teams to capture tester and live user experience to continuously build and deliver high-quality mobile apps.

In a fragmented and complex environment, this service provides quality assurance for your apps, with user feedback and quality metrics available at every stage of app development. This service also includes capabilities for validating apps and tracking production usage.
You can use Mobile Quality Assurance to achieve the following goals:

    Improve the quality of your mobile apps with a holistic visibility into user experience, including bugs, crashes, feedback, and user sentiment.
    Proactively manage quality risks by rapid assessment of issues and reduced cycle time. Listen to user feedback, analyze user sentiment, and use this information to develop a strategy.

Overview of interaction flow between users, Mobile Quality Assurance, and app developers.
The following table describes the roles on a typical team who uses Mobile Quality Assurance and the features that help them to achieve their quality goals.
Role 	Features

Technical app owner
    This role needs to determine how well the app works, how much customers like it, and how to improve the app. A technical app owner can use real-time displays of user sentiment and feedback, including bugs and crashes from testers and users, to reduce defects and improve app ratings.

	calloutlabel 5 User feedback to get feedback about your app straight from your customers.
calloutlabel 1 Sentiment analysis to mine app store ratings and reviews to extract actionable feedback before they go viral.
Rational Team Concert™ and DevOps Services integration automatically records bugs and crashes by connecting to Rational Team Concert.

Mobile app developer
    This role is tasked with building a great mobile application. A mobile app developer can get rich feedback for an existing app.

	calloutlabel 5 User feedback to get feedback about your app straight from your customers.
calloutlabel 4 In-app crash reporting, providing rapid insight into why an app fails.
Rational Team Concert and DevOps Services integration automatically records bugs and crashes by connecting to Rational Team Concert.
calloutlabel 2 Over-the-air app distribution to get the latest content to testers, as soon as it is available.

Tester
    This role goes beyond testing the app function to uncover challenges or flaws in the user experience. A mobile app tester can submit defects and crash logs in seconds while they are using the app from their own device.

	calloutlabel 2 Over-the-air app distribution to get the latest content to testers, as soon as it is available.
calloutlabel 3 Frictionless bug reporting. Submit defects in seconds while you are using the app from your mobile device and automatically log crashes.
calloutlabel 4 In-app crash reporting, providing rapid insight into why an app fails.

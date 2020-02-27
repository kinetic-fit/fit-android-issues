# Public Issue Tracker for the Android Kinetic Fit Mobile Application 2.x Beta

![Kinetic Logo](https://github.com/kinetic-fit/fit-android-issues/blob/master/kinetic_logo.png)
## Getting Started
Thank you for your interest in helping make the Kinetic Fit even better. This private beta test ([opt in here](https://play.google.com/apps/testing/com.kinetic.fit)) will let us test our new version of the app before releasing it to everyone and allow us to smooth out any bugs that are found. For this beta test, we are looking for users who are frequent riders in the Kinetic App (2+ rides a week in Fit) and are willing to do the extra work required to test, report bugs to the issue tracker and work with our developers to reproduce and test fixes for any bugs that are found. Other lower frequency users are welcome to join the beta, but we are asking that anyone in the beta that experiences issues open an issue in the tracker and work with the dev team to fix the issues. We are committed to making Kinetic a better experience and are asking for the same commitment from our beta testers.
 
For the initial round of testing, we are looking for riders to use the Fit app, record their rides and save them. We are also looking to see that your ride data is sharing properly to other services (Strava, Training Peaks, etc) that can be linked in the app. If you have any of the third-party workout apps that Fit can share to, we would appreciate if you would share to those apps and double check that the data is correct. We have not changed the way that we store and serialize the data, but it is always good to recheck these connections and to make sure you can get your data out of Fit.

If at any point you feel like you want to use the public version on the store, you can go back to the opt in link, and follow the directions to remove the beta version from your phone. 

**NOTE: THE BETA DATABASE IS NOT CONNECTED TO THE DATABASE OF ANY OTHER VERSION OF FIT.** You will not be able to access beta workouts in other versions or vice-versa. If you leave the beta and go back to the public version, you will not have access to workouts you did on beta. Because of this, we strongly suggest using a third-party service to save your data. We currently offer connections to Strava, Training Peaks, 2Peak, MapMyFitness, and Google Fit as connections.  
 
## How to Test
When you log into the beta for the first time, you will use your current email and password. The new app will then find your current profile and begin to migrate data over. The new version should immediately pull your profile values over, so your HR zones, power zones, height, weight, and FTP should be set right away. The migration will then go through the last year of workouts you have stored on the old database and bring them over within 48 hours. You will not likely see any history in your main screen for the first day or two. If you do not see your sessions come over after 3 days, please open an issue in the tracker.
 
We will not need specific workouts or features tested by everyone. We should be able to cover all or most of the main features with a large enough pool of testers. The core of the app will always be workouts/free ride, calibration and sharing the data to other apps. Non-core things that can be tested are Custom HUDs, any of the sound options under settings and training plans are all available without a subscription. The Issue Tracker will have a list of the things our internal testers work through, so feel free to touch anything in there if you have the urge. We appreciate any little bit of extra testing we can get.
 
## Reporting Bugs
If you experience an error or notice an issue, please report them in the [Issue Tracker](https://github.com/kinetic-fit/fit-android-issues). This is a public page that we will use to track issues for Android beta testing and will alleviate customer support from tickets that can be opened directly with the developers. (iOS will have its own tracker [here](https://github.com/kinetic-fit/fit-ios-issues).) Please click on the Issues tab under the kinetic-fit/fit-android-issues header. Once there, please search the issues to see if your issue has already been reported. If it has, please add your experience to the issue in a comment. If it has not been reported previously, please open a new issue. No matter how you report, please use the [bug report template](https://github.com/kinetic-fit/fit-android-issues/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) to report your issue to make sure we have all of the information our developers need to get started on your issue.
 
Kinetic is finalizing a new web app, but at the start of this beta you will not have access to it. This means that you will only be able to access your data in the mobile app during the interim. Once this is available for beta testing, we will let you know and you would be free to use the features available there.
 
If you are interested in joining, please go to this [opt-in page](https://play.google.com/apps/testing/com.kinetic.fit) and follow the directions for joining and downloading the beta-version. It may take some time to get the update to your device. If you are having an issue, please go to the issue tracker and search/open an issue. Thank you for your help in making Fit better and for going the extra mile with us.


Please fill out a bug report *for each problem* you encounter. Before creating a report, you should first check the open issues and be certain that it has not already been reported. If it has, please comment with your own experience and the same information required as a new report.

We will do our issue communication here in order to track and organize our efforts on each issue and to avoid confusing issues. Any questions can be sent to kineticbeta@gmail.com or Direct Message to @lexicalninja here on GitHub.

If you need, please review the Test Plan and Test Scenarios documents in the repository to ensure that you understand the requirements for testing and reporting.

## App version 2.4.0 (229) - Feb 25, 2020

This version updates the Garmin FIT library to fix upload errors to third-party sites.
This version also fixes the issue where only one lap showed up on analysis and export of a workout. 

## App version 2.3.4 (228) - Feb 25, 2020

This version looks to try and narrow down the cause of the errors mentioned in the 2.3.3 release notes 
It also attempts to fix a bug in Profile deserialization when syncing. 

## App version 2.3.3 (227) - Feb 20, 2020

Some user's may be experiencing crashes when exporting to Strava or other apps. There is currently an issue in the app during deserialization causes a Concurrent Modification Exception. This version looks to either fix or significantly reduce those issues. 
Fixes a bug on the sensor setting screen. If you tapped an icon to disconnect as a type of sensor, it would disconnect as that sensor, then immediately reconnect but leave the icon gray. which isnt very helpful. This should fix that.
This version should fix a bug that causes users to get a "Kinetic Crashed" error when the app has been backgrounded and not in use.

## App version 2.3.2 (226) - Feb 5, 2020

This version cleans up issues that caused crashes in a small number of sessions. The majority of the bug fixes dealt with random single crashes that most likely occurred during a workout session.
This version also fixes a bug that crashed users on the select category screen, and one that crashed users on the profile screen.

## App version 2.3.1 (225) - Feb 3, 2020

This version fixes a bug on the Sensor Settings screen that always showed kph for speed sensor value, even if user is not metric.
This also fixes a major crash when a user starts a Training Plan, as well as other UI fixes for the TP calendar view.

## App version 2.3.0 (224) - Jan 30, 2020

This update adds an overlay when connecting to a sensor to ensure all FTMS services have been processed and that the sensor is ready for changes or input/output. 

## App version 2.2.0 (223) - Jan 24, 2020

This update removed subscription features from the app. These have been removed for the public beta and will be reintroduced once the app leaves beta.

## App version 2.1.3 (222) - Jan 23, 2020

This update makes changes to fix the bug where imperial/metric settings were not being saved correctly between sessions.

## App version 2.1.2 (219) - Jan 2, 2020

This update makes changes to the migration process and to the Profile object to ensure that the preferred units of measurement are saved for the user when they migrate, as well as making sure they save to the server correctly when the user changes it.

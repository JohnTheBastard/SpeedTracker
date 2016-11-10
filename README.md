# SpeedTracker
SpeedTracker is an app to display your current speed as well as average speed, time,  and distance travelled, over the course of a run, drive, or bike ride. Your route is displayed on a map in real-time and aggregated with past routes so the user can see their statistics for time spent driving, average running speed, or the total distance travelled biking over their usage history.

SpeedTracker is for anyone who is looking to track their daily runs or commute time, or simply wants a speedometer for a bike or motorcycle that doesn't have one. The app helps the user by doing much of the work for them. By simply selecting walking, biking, or driving as their choice of transportation upon opening the app, SpeedTracker will tailor the data collection to best suit that type of travel. From there, the user is taken to the route view where they can begin and end their route and see real-time data about their trip. Once the user clicks the End Route button, their data  will be saved locally (as well as in the cloud if the user has an iCloud account enabled) and used to tabulate total distance, total travel time, average speed, average distance as well as total routes completed for each respective mode of transport.

The user can swipe down on the route view or press the Dismiss button to return to the previous screen to select a new mode of travel, or select the Stats tab to see their cumulative data.

The following frameworks we used to build this app:
-CoreLocation
-MapKit
-CloudKit

Implementation Details:
We worked mostly with Core Location while building this app. It was useful for requesting location services/authorization, selecting the desired location accuracy and type of transport, gathering the current speed,  and deciding how often to regenerate data; to name a few. MapKit was used for displaying the user's location and drawing the user's route on screen. While user data is stored locally on their device, CloudKit is used as a backup as well as means to synchronize travel history across all of user's iCloud-enabled devices.
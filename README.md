# Swaasthy
## A Google DSC Solution Challenge submission

![hero](https://user-images.githubusercontent.com/65770068/160841669-96839e12-d502-4c8d-b44a-1101f32cd508.png)

Swaasthy is an app made to uplift user's health. It contains everything from medicine reminder functionality to make an SOS call to nearby ambulances to getting an appointment with a virtual doc. We believe that this is a revolutionary step necessary in bringing down the death-rate due to delay faced by patients in our country.

## Project Info
The contents in this project follow the following structure, where all views are containerised into screens.

├───models
|
├───screens
│   ├───auth
│   ├───consult
│   ├───emergency
│   ├───forums
│   ├───home
│   ├───reminder
│   └───stats
|
├───services
│
├───shared_widgets
│
└───utils

Each individual screen in the above, follow this structure
screen
  ├──local_widgets
  └──index.dart

## Constants
This project uses 'Product Sans' as it's primary font, with weights of 400 and 600. All the fonts have been pre-imported.

Moreover, here are a few constants which are used throughout the project, and have been added within a CodeRedColors class, use them accordingly.
base            : FAFAFAF
primary         : EE466E
primaryAccent   : bd284b
inactive        : 9E9E9E
primary2        : 6246EE
primary2Accent  : 3a21b8
inputFields     : F3F3F3
medicineCard    : FDA8F3
text            : 000000
textSecondary   : 828282

## Designs
All the design/mockups for the app have been added in the designs directory. You can use those for reference.

## Description
!. Our solution mainly consists of a Flutter based mobile app. We wanted our solution to reach the masses, that's why we picked flutter as our framework of choice because of its cross-platform capabilities.

2. For the backend, we mostly relied on Firebase, as it was easier to integrate with the flutter app, without any hassle to manage & create instances of our server.

3. For sign-up & authentication, we used Firebase auth. If you're a medical volunteer, we'll ask you to upload an image of your medical ID card and we're using firebase ml kit for verification.

4. For storing the different types of data including user data, posts for the forum, ambulances, insights for the heatmap, doctors, appointments etc. we chose Cloud Firestore because of its robust features and ability to query & filter out documents with ease.

![1](https://user-images.githubusercontent.com/65770068/160841767-c4944eaa-29d9-41b8-a63e-e697d9d1a080.png)
![2](https://user-images.githubusercontent.com/65770068/160841794-7af47b0e-9034-4747-8f1f-2f6cd89b15f3.png)
![3](https://user-images.githubusercontent.com/65770068/160841825-5e9c7a4b-db5f-48dd-8a44-519072ba5f1b.png)
![4](https://user-images.githubusercontent.com/65770068/160841852-efb6e6c3-fcf7-4bf2-89af-9ac8f46b17bd.jpg)
![5](https://user-images.githubusercontent.com/65770068/160841881-a44ec6c1-4cfd-4a92-8e70-7898bf7a3a19.png)


5. For verifying the medical volunteer ID Card Image, we used Firebase ML Kit, specifically the text recognition service.

6.To enable image posting in forums, and to store the volunteer image we used firebase cloud storage.

7. For handling payments, we used Razorpay SDK, which allowed us to accept payments for doctor appointment booking using Google Pay.

8. Adding video-calling for doctors and users was a challenging part, we ended up using agora WebRTC SDK to enable that feature within the app.

9. For the symptom-based disease recognition system, we looked up a lot for a reliable resource and ended up using prepaid service from ApiMedic.

10. For the Google Assistant Action, we used actions SDK with Google Actions builder tool, along with that for hosting an instance for webhooks, we used GCP.

## Setup
Clone the repository
git clone https://github.com/ishandeveloper/Google-DSC-Solution-Challenge.git

# Move to the desired folder
cd \Google-DSC-Solution-Challenge

# To run the app, simply write
flutter run

## About
Solving real-life problems is not easy, but at the same time, it's not impossible. Keeping this in mind, a team of four student developers from Chitkara University, Punjab, worked throughout March to solve a concerning problem by leveraging tech.

Our app primarily deals with the health sector. When it comes to saving a life, every millisecond counts! One in 10 patients in India dies on the way to the hospital. And we're here to change to that. We're Swaasthy!



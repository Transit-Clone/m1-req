# **Pathly**

**Team Members**: Sammi Chong, Ellie Lu, Naseeha Masub, Saba Sohail @ Stony Brook University  

---
## **Project Overview**
Our project's goal is to develop a mobile public transportation app called **Pathly**, inspired by existing apps like Transit, Citymapper, and Google Maps. Like other transit apps, our app will allow users to search for transit routes, view nearby stops, compare routes, and navigate to their destinations using real-time and scheduled transportation data. The system will integrate publicly available transit data with mapping services to provide users with an intuitive interface for planning trips.

---

## **Problem Statement**
Even though there are countless public transportation apps already out there in the market, riders often express frustration with issues like:

- cluttered UI
- inaccurate bus/train times
- incorrect routes
- lack of support for [intermodal passenger transport](https://en.wikipedia.org/wiki/Intermodal_passenger_transport)
- paywalled features

Because no single application consistently addresses all of these issues, riders find themselves juggling multiple applications at once or being forced to pick one despite its many flaws. For example, existing apps have their own strengths and limitations:

| Application | Strengths (+) | Limitations (-) |
| -------- | -------- | -------- |
| Google Maps | best map interface | requires destination input |
| MTA App | updated interface since March 2026 | still lackluster and unintuitive |
| Citymapper | best route navigation | cluttered home UI, restrictive search |
| Transit | best UI overall | paywalls core features |

While these apps are certainly popular and provide useful services, their differences mean that users are forced to compromise between UI, route accuracy, and available features. These concerns are especially evident in Google Play ratings and reviews:

| Application | # of Downloads | Rating | Example Review |
| -------- | -------- | -------- | -------- |
| Google Maps | 10B+ | 3.2 | "cant get MTA transit info unless you put in the address of where you are going...sometimes you want to know nearby transit...Without typing the destination." |
| MTA App | 1M+ | 3.1 | "You guys took a simplified platform and overcomplicated it beyond comprehension. Time is of the essence...It is so hard to navigate..." |
| CityMapper | 10M+ | 4.8 | "I just keep getting confused or not getting the right information I need." |
| Transit | 10M+ | 4.6 | "...loved this app until the most recent update, which completely changed the ui and...functions...it's harder for me to tell which bus I am taking and when it will arrive." |

Clearly, even though these apps already exist, there is still a need for a solution that is accurate, reliable, efficient, and intuitive.

---

## **Target Audience**
Over 4 million NYC residents and 400,000 Long Island residents use public transit everyday. In NYC, roughly 49% use public transit (the highest in the U.S.) and 56% do not own a car. Obviously, pubilc transit is essential to NYC and LI.

As such, our app is created for individuals that rely on public transportation in these areas. This includes both new and experienced riders who travel for work, school, leisure, or any other reason.

Due to the lack of transit app data from users, we conducted a survey to better assess our target audience. However, most of our respondents were SBU students, so our results may not accurately represent the entirety of the NYC/LI population. Based on our survey of 25 respondents, 85.7% reported using multiple transit apps to navigate and 47.6% reported inaccurate arrival and departure times. Clearly, this is a relevant issue for riders as mentioned earlier.

Additionally, after analyzing ridership numbers, we determined that our app will cover the following systems:

- MTA Bus
- MTA Subway
- NYC Ferry
- LIRR
- Nassau Inter-County Express
- Suffolk Bus Transportation

We will implement the last 2 systems if time permits for Long Island residents.

---

## **Our Solution**
We want to create a mobile app called Pathly that provides users with an all-in-one platform for all of their public transportation needs. It will keep the features that users love about their existing apps while adding others that are useful and intuitive. For example, users will still be able to view arrival times, see routes, and search for destinations, but our app will have better accuracy, UI design, personalization, and other features for an enhanced user experience.

We aim to reduce the need for users to switch between different apps to navigate by prioritizing comprehension and detail without being overwhelming. The app will present relevant trip information clearly and allow them to access additional details when needed. Our initial version will primarily focus on public transportation services within New York City and Long Island with a hope to expand to other cities in the future.

---

## **Why a Semester**
Designing a unique and reliable public transportation app is not a straightforward process, it requires many iterations. Even if AI is able to create most of it for us, it is very likely that we may have to change or add certain features to better accommodate users. Due to a lack of online data about public transit apps and user preferences, AI alone will not be able to sufficiently determine user needs without specification.  

This application requires combining multiple NYC and Long Island transit APIs, each with different data formats and update speeds. It also needs complex route calculations based on time, cost, walking distance, transfers, and user preferences, while handling edge cases such as delays, cancellations, and missing data. Additionally, real-time locations, schedules, service updates, and automatic rerouting require extensive backend development, testing, and optimization to ensure the app works reliably.

Additionally, despite there being many public transportation apps out there, very few users actually use them. Most use the default apps like Google Maps or official apps like TrainTime. Of our 21 respondents, only 8 of them (38%) said that they used apps other than Google Maps, Apple Maps, or any other official apps. As such, there is a known challenge in creating a transit app that people are willing to give a try. It needs to be significantly better than existing apps. Our plan is to incorporate features that people enjoy using into a single convenient app.

---

## **v1 Scope**
#### **In Scope**
Our app will provide users with an easy-to-use interface that allows a variety of functionality. Most importantly, users can:
*   View bus/train routes
*   View GPS location of bus/train
*   View schedules
*   View frequent and previous trip details
*   View fare cost
*   Search for destination
*   Find routes to get from A to B
*   View service delays/changes
*   Save trips, stops, and locations
*   Set alarms for their next stop
*   Set route/mode preferences (less walking, cheapest, fastest, etc.)
*   Automatically redirect users in the case of delays/service changes
*   Create personalized widgets to show times
*   Add friends
*   Personalize their profile/icon

#### **Out of Scope**
*   Redirecting users to buy tickets
*   Seeing other users' location
*   Support for other transportation systems outside of NYC/LI

---

## **User Stories**
- As a commuter from LI to NYC, I want to have one trip that lists all forms of transportation so that I don’t have to manually combine routes myself (ex: LIRR -> NYC Subway -> Walking -> NYC Bus)

- I want to see the grand total of fare costs, maybe one trip is cheaper than the other? I also want to compare trip times, maybe one trip is shorter than the other?

- As a NYC subway commuter, I want my location accurately tracked in between stations or stops underground (offline), so I don’t miss my transfer or get inaccurate information

- As an infrequent, or directionally challenged, NYC commuter traveling through Grand Central or Penn Station, I want step-by-step guidance when stepping off the train

- As a late-night, or sleep deprived, commuter,  I want my phone to alarm me as I reach my next transfer so I can nap during my ride without missing my stop

- As an experienced rider, I want to view my bus/train times and GPS location immediately when  I open the app so that I can easily catch it without wasting time.

- As a rider, I want to search for a destination so that I know how to get there using public transit.

- As a rider, I want to compare multiple routes so that I can choose the option that best fits my needs.

- As a frequent user, I want to save my favorite routes/stops so that I don’t have to search for them later.

---
## **Team Roles**
Each team member will have a primary area of responsibility, while UI/UX design will be a shared responsibility across the entire team.

| Team Member | Responsibility | Tasks |
|---|---|---|
| **Sammi Chong** | frontend | Implement the main application pages and user-facing components, including the home screen, search interface, route results, navigation interface, and frontend integration with backend endpoints |
| **Ellie Lu** | backend / server | Develop server-side logic, create backend endpoints, handle requests from the frontend, process route and user data, and help integrate external transit data sources |
| **Naseeha Masub** | backend / server | Develop server-side logic, create backend endpoints, handle transit API/data integration, process route and arrival information, and support communication between the frontend and database |
| **Saba Sohail** | database | Design and manage the database, create data models for users, saved locations, pinned trips, and trip history, and support persistent application data |

---

## **Functional Requirements**

### **1. User Authentication**

### What
Users can create an account, log in, and log out.

### How
The user's session should remain active while they use the application. User-specific information should be connected to their account.

### Demo
1. Create or log into an account.
2. Save a destination.
3. Log out.
4. Log back in.
5. Verify that the destination is still saved.

---

### **2. Home Screen**

### What
The home screen gives users quick access to transit information and trip planning.

### How
The home screen should contain:

- Search bar
- Map
- Nearby transit options
- Saved/frequent destinations
- Recent destinations
- Profile/settings button

### Demo
The user should be able to open the application and immediately begin searching for a destination.

---

### **3. Destination Search**

### What
Users can search for where they want to go.

### How
The search page should allow users to enter a location or destination and select a result.

Search should be fast enough to realistically use while commuting.

### Demo
Search for a destination such as:

`Stony Brook University`

and select it from the results.

---

### **4. Route Planning**

### What
The system returns possible public transportation routes between an origin and destination.

### How
Each route result should display at least:

- Transit mode
- Route or line
- Estimated trip duration
- Departure information
- Number of transfers

The application should support trips involving multiple transit systems when possible.

### Demo

Example:

`Stony Brook → Penn Station`

The application returns one or more possible transit routes.

---

### **5. Route Details**

### What
Users can view the individual steps of a selected route.

### How
The route should be displayed as an ordered sequence.

Example:

`Walk → Suffolk Bus → LIRR → Subway → Walk`

Each step should tell the user where to board, transfer, or exit.

### Demo
Select a route and display its complete list of trip steps.

---

### **6. Route Map**

### What
Users can view the geographic path of their trip.

### How
The selected trip should display relevant stops and routes on a map.

### Demo
Select a route and display the route geographically.

---

### **7. Transit Times**

### What
Users can see relevant arrival or departure information for their trip.

### How
The application will retrieve real-time information where supported by the available transit data source and scheduled information where real-time information is unavailable.

The interface should make it clear what time the user should expect the vehicle to arrive or depart.

### Demo
Display departure or arrival information for a selected transit route.

---

### **8. Saved Stops and Destinations**

### What
Users can save frequently used locations.

### How
Saved locations should be stored in the database and associated with the user's account.

### Demo
1. Search for a destination.
2. Save it.
3. Refresh or reopen the application.
4. Verify that the saved destination still appears.

---

### **9. Recent Searches and Trip History**

### What
Users can revisit previously searched destinations or trips.

### How
Previous trips should be stored for the user's account and displayed in reverse chronological order.

### Demo
Search for a trip, leave the page, and retrieve the trip again through the user's history.

---

## **10. Pinned Trips**

### What
Users can save important trips for future use.

### How
Pinned trips should remain associated with the user's account until the user removes them.

### Demo
Pin a trip and verify that it remains available after leaving the page or starting another session.

---

### **11. Stop Alarm**

### What
Users can set an alarm for an upcoming stop.

### How
While viewing a trip, the user should be able to choose an upcoming stop and enable or disable an alarm.

### Demo
Select a stop from an active route and enable its alarm.

---

### **12. Profile / Settings**

### What
Users can access their account information and settings.

### How
The profile/settings page should provide access to:

- Basic account information
- Saved destinations
- Saved/pinned trips
- Trip history
- Application settings
- Logout
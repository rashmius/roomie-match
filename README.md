
# Roomie Match 

## Objectives

1.	Develop a user-friendly interface that allows users to connect and match with potential roommates easily.
2.	Put in place a robust algorithm for matching roommates.
3.	Allows for customizing user profiles by adding summary, hobbies, stream, cleanliness requirement, budget, location, etc.
4.	It has a chat interface for communicating with matched users.
5.	Has a feedback system to capture more insights & improvement areas in the application.

## Functional Requirements

1.	User Profile Creation
   
  a.	Users must create their profile & without profile features - roommate search, chat will not be accessible.

  b.	Users can't change their registered mail address and will be tied to mySlice logged-in email address.
  
  c.	The user's age will be auto-calculated and can't be modified. It will be pulled from mySlice information database.
  
  d.	Users can add and change their preferences for the fields made available by the admin.

  e.	Users must add mandatory fields configured by the admin, and can't be left empty.
  
 
3.	Roommate Search
  a.	Users request candidates to send connection requests to; results will be listed for pairs found by the algorithm.

  b.	Users can add/remove filters to finetune the search.
  
  c.	Search to limit by top 10 users.
  
  d.	Currently, users can request unlimited searches, but implementation supports limitations for the future paid model.
  

5.	Sending and Receiving Roommate Connection Requests
   
  a.	Users can send a connection request to the received output from the search.

  b.	Users will be notified upon receiving a connection request via registered email.
  
  c.	The email will include a redirection to the application to view the connection request.
  
  d.	The receiver can view the entire profile of the sender.
  
  e.	The receiver can either approve or reject the request.
  
  f.	The sender will be notified when the receiver accepts the request.
  
  g.	The number of connection requests a user can send will be unlimited as of now; implementation to support limitations for the future paid model.
  

7.	Chat
   
  a.	Receivers, only once accepting, can chat with the sender.

  b.	Chat can be done from both sides.
  
  c.	Both ends will be notified by push notification on receiving a text.
  
  d.	Text will be limited to 1000 characters.
  

9.	User Feedback and Ratings
    
  a.	Feedback popup will be shown to users every time a user has been engaging in chat for a day with another user.

  b.	The feedback popup will contain a star-based rating system ranging from 1 to 5. This field will be mandatory
  
  c.	The feedback popup will also contain a text area to enter detailed feedback. This field will be mandatory.
  


## Non Functional Requirements


1.	Privacy
   
  a.	User data should be secured with industry-standard encryption.

  b.	User consent before collecting engagement data
  
  c.	Data deletion requests can be taken with the agreement of 30 days.
  
  d.	Data sharing with third parties (for example - housing providers) will be disclosed before and requires explicit consent while registering.
  
  e.	Users can opt out of data sharing with external third parties.
  

3.	Availability
   
  a.	Minimum uptime of 95% of the roommate services.

  b.	Application monitoring to identify failures and plans to mitigate them should be made.

  c.	Maintenance/Downtime periods will be at night, from 12 am EST to 5 am EST, which can be of any duration.
  
  d.	Application status is to be made available and integrated with mySlice status page.

5.	Performance
   
  a.	Maximum response time of search feature of 5 seconds.

  b.	Maximum response time of other requests of 2 seconds.

  c.	The application should be able to handle 100 parallel searches on the matching algorithm and a minimum of 1000 users load per second.
  
 
7.	Usability
   
  a.	The application should have a consistent design across all pages and functionalities.

  b.	Error messages should be present in case of any failures in the system.
  
  c.	Error popups are to be present throughout the application to minimize user errors.
  
  d.	Application documentation will be present on MySlice website only, with a FAQ section to guide users.
  

9.	Compatibility
    
  a.	Support all browsers supported by MySlice, such as Google Chrome, Firefox, and Brave.

  b.	Support all mobile devices of various screen sizes, which mySlice supports.
  


11.	Maintainability
    
  a.	Maintenance will be performed as per existing MySlice maintenance schedules.

  b.	Support will only be provided by email with documentation and FAQ on MySlice website.
  


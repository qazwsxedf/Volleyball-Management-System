Software Requirements Specification
1. Introduction
1.1 Purpose 
The purpose of this document is to present a detailed description of the Smash or Pass website. It is used to centralize tournament and drop-in management for a volleyball community that currently uses Discord, Google Forms, and Google Sheets.

1.2 Scope
This website will be for a local volleyball community. It is designed to make it easier for users to find and sign up for volleyball events. It is designed to allow organizers to create and manage events, such as tournaments and drop-ins, and to allow admin to post news about the events and the community. 
1.3 Background / Problem
Currently, communication about tournaments and drop-ins are done through Discord. To register for drop-ins, a Google Sheet is shared where users can input their names, as well as display other information such as status (Coming, Not Coming, Maybe Coming), payment status, and details about the session. For tournament registration, individuals sign up their team either through Google Forms or by reaching out to the admins directly. The admins then post the list of teams, the schedule, and the rules in a google sheet that is shared with teams and players.

I would like to combine the information in one easy to access and use website, where users can easily organise and join games and drop-ins. For drop-ins, organizers can place players in teams beforehand if they decide and the teams will be displayed for the players to see. For tournaments they can also add and remove teams.
2. Overall Description 
2.1 System Environment 

Users can have multiple roles.
2.1 Player
Players are able to register individually or a group of people for drop-ins, or a team for tournaments.

2.2 Organizer
Same abilities as players, plus they can organize and post drop-ins and tournaments for other players to join, and edit them after creations. Can create teams in drop-ins and add and remove teams for tournaments.

2.3 Administrator
Same abilities as the others, plus they can manage users, events, and posts on the homepage.








3. Functional Requirements 
3.1 Authentication 

Functional Requirement 
Functional Requirement Narrative 
FR-AUTH-001
The system will allow users to register an account 
FR-AUTH-002
The system will allow users to login to existing account with correct username and password
FR-AUTH-003
The system will allow authenticated users to log out of their account 

3.2 Events
FR-EVENT-001 — View Upcoming Events 
Requirement:
The system shall allow all users to view upcoming events and event details 



Functional Requirement 
Functional Requirement Narrative 
FR-EVENT-001
The system will allow all users to view upcoming events and event details 
FR-EVENT-002
The system will allow approved users to create, edit, and cancel events
FR-EVENT-003
If an event is full, users will be put on a waitlist

3.3 Tournaments 

Functional Requirement 
Functional Requirement Narrative 
FR-TOURN-001
The system will allow authenticated users to register for an upcoming tournament
FR-TOURN-002
The system will display the current number of registered players/teams for a tournament
FR-TOURN-003
The system will allow organizers to manage the teams registered for the tournament



3.4 Drop-ins

Functional Requirement 
Functional Requirement Narrative 
FR-DROP-001
The system will allow authenticated users to register for an upcoming drop-in
FR-DROP-002
The system will display the current number and names of registered players for a drop-in
FR-DROP-003
The system will allow organizers to manage the players registered for the drop-ins

3.5 Organizer Management

Functional Requirement 
Functional Requirement Narrative 
FR-ORG-001
The system will allow authenticated users to request to become an organizer
FR-ORG-002
The system will allow admin to approve request to become organizers
FR-ORG-003
The system will allow organizers to create events

3.6 Administration

Functional Requirement 
Functional Requirement Narrative 
FR-ADMIN-001
The system will allow admin to view pending requests
FR-ADMIN-002
The system will allow admin to approve/reject requests
FR-ADMIN-003
The system will allow admin to post announcements 
FR-ADMIN-004
The system will allow admin to manage events 




4. Non-Functional Requirements 
Should work well on mobile 
Passwords safely stored 
Code should be appropriately separated
Pages should load reasonably fast 






































5. Business Rules 
A user must create an account to register for an event

A user must request to able to organize events and this request must be approved by an admin

A user may have multiple roles (player, organizer, admin)

Only organizers assigned to an event can modify the event

An event cannot accept registrations after its registration deadline

A players status will only be marked/shown as paid once the organizer marks it as so

Listings will only stay up for a week after they have happened



































6. User Flows / Use Cases 










































7. Data Requirements 
User
User_id
Username
Roles
Email
Password

Tournament
Tournament_id
Name
Date
Time
Address
Registration deadline
Capacity 
Created_date
Organizers

Drop-ins
Date
Time
Address
Capacity
Registration deadline
Created_date
Organizers

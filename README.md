# Final_Project

## PROJECT PROPOSAL

<br> 

#### 1.0 Introduction

> A hotel reservation system is a necessity for today’s accommodation providers as the reservation system enables users to book a hotel room with a cohesive system where it allows users to navigate the system by adding, filling and searching a hotel and the room based on their preferences. As well, it allows the users to book the hotel room online and the system encompasses the hotel’s availability resources such as Wifi, Pools and Breakfast. Furthermore, the system provides multiple pictures for each hotel room. Other than that, it validates the users to schedule dates and length of stay.

#### 2.0 Objective
 
   <ul>
  
   <li>Allow users to look for personal references in hotels.</li>
   <li>Allow the system to display the hotel availability.</li>
   <li>Able users to navigate the system in terms of filling form and searching.</li>
   <li>Allow users to delete booking reservations.</li>

   </ul>

#### 3.0 Features and functionalities

   <ul>
   <li>Associate every online booking </li>
   <li>Enable users to search and find the most relevant booking options</li>
   <li>Accept date and time to check available rooms for that particular time</li>
   <li>Booking confirmation should be sent to the specified contact details</li>
<li>Calculate and display accommodation charges and other utilities</li>
<li>Cancel bookings</li>
<li>Display and change records of guests</li>
</li>
   </ul>
 
#### 4.0 Entity Relationship Diagram (ER Diagram)

<br>

**Views :**

   <ul>
   <li>home.blade.php : DDisplays various hotels’ room availability and a Home page</li>
   <li>bookingform.blade.php : Displays a form for users to book a hotel’s room.</li>
   <li>showbookform.blade.php : Displays User details on booking the room and displays a book room detail page with edit and delete button for cancelation.</li>
   <li>Index.php until index6.php : Display available hotel’s room.</li>
   </ul>
   
<br>

**Controllers :**

   <ul>
   <li> roomsController.php :</li>
   <ul>
   <li> Allows booking room form passed into the database.</li>
 <li>Allows booking room form data to be updated.</li>
 <li>Allows booking room form data to be removed from database</li>

   </ul>
  
 <br>

**Routes :**

   <ul>
   <li>Route::get('/bookingform', [App\Http\Controllers\roomsController::class, 'index'])->name('rooms'): Route for return return data passed rooms form which roomsController.php into view.
</li>

 <br>
 
**Models :**

   <ul>
   <li> Booking.php : user has one-to-many relationship with booking room (a users can book many rooms)
</li>
   <li> Room.php : room has one-to-one relationship with user ( one book room has one user)
</li>
 
   </ul>
   
<br>

**User Athentication :**

   <ul>
   <li> User update room booking (cancel/change).
   </ul>
 
 <br>
 
 **Entity Relationship Diagram :**

<br>

![Entity Relationship Diagram](/resources/ERD.png)

<br> 

#### 5.0 Sequence Diagram

<br>

![Entity Relationship Diagram](/resources/SD.jpg)

<br>

#### 6.0 References

    Internet Booking Engines   https://www.siteminder.com/r/technology/hotel-internet-booking-engines/requirements-hotel-reservations-system/

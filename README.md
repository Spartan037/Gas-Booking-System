# Gas-Booking-System

<h2>Package GAS SUPPLIER</h2>
<br>•	Define an interface Gas agency which is having  Agency name, agency code, phone number ( all are final variables). With the display method.

<br><br><h2>Package CUSTOMERS</h2>
<br>•	Customer class is  having details like  name, mobile number  address ( street, area,  pin code) 
<br>•	Gas connection class is inherited from the customer class is having connection number (should be  sequential number which is automatically generated (use static)), number of cylinders, Last booking date (current date is the last booking date while creating object). 

<br><br><h2>Package GASBOOKING</h2>
<br>•	Booking is the another class which records the cylinder booking details  such as Gas connection number, Booking date,OTP, Amount, Status( B-Booked (during booking) , D-delivered, C-Cancelled, P-Pending) While booking validate that booking date could be 30 days from the last booking date for the single cylinder holder and 50 days for the two cylinder holder. If not booking cannot be done. If booking is done , update the last booking date  in the gas connection class. After 7 days from the booking date that status is updated to (P-Pending)
<br>•	Define another class Delivery which is uses the information Gas connection number, Booking date, OTP  from the booking class and have  additional details like delivery date and the delivery person name.
<br>o	While creating object for delivery person ask for the gas connection number, fetch the booking date and OTP form the booking class objects (whose status is B or P). 
<br>o	While delivery, the delivery person should ask for the OTP to the customer ( accept from the user). If the OTP given by the customer is matched with the OTP generated while booking, then only  cylinder will be delivered and update the status in the booking class as  (D-delivered ) else cancel the process and update the status as (C-Cancelled ).  Validate that the gap between the booking date and delivery date should be between 2 to 7 days.  If it exceeds 7 days, then 5% of the cylinder should be refunded to the customer. Update the amount in the booking class.

<h3><br><br>Define methods in the appropriate class and Use constructors wherever is required</h3>

<br>1.	Display how many cylinders are delivered on a particular area in a given month.
<br>2.	How many cylinders are delivered late in a month ( check the amount in the booking  class)
<br>3.	Display the name and mobile number, gas connection number who got single cylinder connection.
<br>4.	Display the customer name address for which particular delivery person is delivered the cylinder. (Accept the delivery person name from the user).
<br>5.	Print the report 
<br>  <p> &emsp;a.	All delivered bookings
<br>  &emsp;b.	All pending bookings
<br>  &emsp;c.	All cancelled bookings
<br>  &emsp;d.	All delivery person details.</p>

<br>6.	Print the invoice in the following format

<br></p>Gas agency code:XXXXX     &emsp; Date of Invoice : ( Current date)                                                                                                                                                                                                                                                                                                                                                                                                      ,
<br>Gas Agency name:XXXXX		&emsp; Gas Agency Phone number : XXXXX
<br>Gas connection number:		&emsp; Customer Name:
<br>Booking Date:			&emsp; 	customer: mobile number</p>


<br><br>Amount :
<br>Refund :
<br>Total Amount:

<br><br><p>Delivery Person Name :xxxxxx			&emsp; Delivery  Person Phone number :XXXXXX
<br>Delivery date :XXXXXXX</p>



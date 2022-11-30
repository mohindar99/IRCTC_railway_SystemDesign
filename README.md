# IRCTC_railway_SystemDesign

## Introduction :
In this system design we are going to know about the complete structure of the Indian railway system and its working .
Some of the main criterias of this system comes under these parameters .
- Search Train 
- Book Train
- Cancel train 
- User Notification

## DataBase Structure:
In this architecture we mainly use the relational database as it is highly structured and maintained easily .
Some of the relational data bases which we probably use in this system are:
- Train_details
- Booking_train
- Train_booking_details
- User_database
- Payment_database

## Important API's :
**User Services** 
   1. Create User(userid,password)
   2. Post User Details(user details)
 
**Train search service**
   1. List Train(from ,to , date,quota ,class)
   2. getTrain Route(TrainNum , date)

**Book Ticket Services**
   1. Generate PNR()
   2.BookTicket(train detail , userDetails)
   
**Payment Services**
   1. PaymentProessing (PNR , transactionID, payment type)
   2. Initiate Payment(PNR ,transaction ID)
   3. Initiate Refund (PNR , transaction ID)
   
  **Notification Service**
  1. SMS ticket
  2. Email Ticket
  3. Notify train running status(ticket)

## Capacity Estimation:

 1. Train details/month - 6.2gb
 2. Train_booking_info & Details/month - 8gb
 3. Booking_payments_details/month - 4.6gb
 4. Total size/month - 18.8gb
 5. Total size/year ~ 223gb
 6. Total size/5 years ~ 1 Tb
 

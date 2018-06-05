# hotelbooking

HotelBooking application Details:

Prior requirements : Mongodb is required to be started in port number 27017.

Steps to run the application command line:
	Download the hotelbooking.zip file from GIT Repository location (https://github.com/jsnrao/hotelbooking)and extract the folder in your system.
	Go to hotelbooking/target folder and run the below command to execute the application.
		java -jar hotelbooking-0.1.0.jar Application

Steps to import to eclipse and run the application
1) unzip the hotelbooking folder to the computer
2) In Eclipse/STS import the project as an existing project
3) Right mouse click the project select configure and select convert to maven project
4) Run as maven install 
5) Run as Spring boot application

Once the applciation starts successfully we can access Swagger-ui using the below url
	http://localhost:8095/swagger-ui.html

Application functionality: Booking Repository contains the Hotel and Customer details. Without Hotel and Customer we cant book the hotel.
	We can add/delete/update/findall/findById api's implemented for Customer/Booking/Hotel entities. Implemented the test scenarios for the same.
	Notification service implemented but as we change the SMTP details we can validate other wise we can not validate. Added smtp properties in application.properties. Notification code has been commented in bookingServiceImpl class save and update methods. If all the properties are correct
	notification will be sent on success or failure of the booking.
	
	
Build:
Utilized pom.xml for maven configuration and gradle files as well for building the application.

Application Contains below controllers:#
1)HotelController
2)Customer Controller
3)Booking Controller
4)Notification Controller

Application contains the below services:
1) HotelService 
2) CustomerService
3) Booking Service
4) Notification Service

Entities:
1) Booking
2) Customer
3) Hotel

Repositories
1)HotelRepository
2)CustomerRepository
3)BookingRepository

Test Cases:
1)CustomerControllerTest.java
2)BookingControllerTest.java
3)HotelControllerTest.java
4)CustomerServiceTest.java
5)HotelServiceTest.java
6)BookingServiceTest.java


All the application properties are placed in application.properties
It is using Junit5 testcases for the controllers and Services using Mocking.

Below, you can find the description of your eighth assignment, which also
includes its output in the Application Walkthrough section.
In this assignment, you are expected to improve your existing Hotel
Reservation System by incorporating Comparator and Comparable interfaces.
It is imperative to create a class named CostComparator, which implements the
Comparator interface and employs the getCost() method of Services to sort the
overall cost per service in a descending order.
In addition, the reservations should be sorted in ascending order by using their
hotelName attribute. To accomplish this, you need to define the Reservation
object as Comparable by implementing the Comparable interface.
When the application starts, it should prompt the user with the following
menu:
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
On top of the existing options implemented as part of the previous assignment,
this one introduces 2 more menu items, whose functionality is described below.
When the user selects the 10th option, the system is expected to arrange the
services based on their total cost using the CostComparator class. In this class,
the Comparator interface must be implemented with the type of objects that
may be compared by this comparator, which is the Services class. Thereafter,
the compare(Services o1, Services o2) method must be overridden to compare
the overall cost of the two Services instances. The sorting process will require 
the system to traverse through the calculableList, which additionally to other
calculatable objects, it also contains all the services. After identifying the
Services type instances, these objects must be added to a temporary arraylist.
The Services objects in this arraylist must be sorted in descending order
according to the result returned by the getCost() method. To display the
information about the sorted version of these services, a method named
displayServiceInfo() must be implemented in Services class. This method
should provide details such as customerID, getServiceType() and
calculateService().
When the user selects the 11th option, the system is expected to arrange the
reservation hotel names in an alphabetical order and display their service
information – utilizing displayServiceInfo() method. Initially, you must declare
that you are going to implement the Comparable interface in the Reservation
class and then override the compareTo(Reservation o) method as you need. The
sorting process requires iterating over the calculableList and identifying
instances of the Reservation, which must be subsequently added to a
temporary arraylist. The Reservation objects in this arraylist must then be
sorted in alphabetically ascending order based on the hotelName attribute. The
resulting sorted list must then be printed on the screen by calling the
displayServiceInfo() method.
Application Walkthrough
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
1
ROOM INFOS:
Room Type: Single, Daily Cost: 100, Room Size: 15, Has Bath: false
Room Type: Double, Daily Cost: 180, Room Size: 30, Has Bath: false
Room Type: Club, Daily Cost: 250, Room Size: 45, Has Bath: true
Room Type: Family, Daily Cost: 400, Room Size: 50, Has Bath: false
Room Type: Family With View, Daily Cost: 450, Room Size: 50, Has Bath: true
Room Type: Suite, Daily Cost: 650, Room Size: 80, Has Bath: true
Hotel Name: Hilton Istanbul
Room Type: Family
Reservation Month: April
Reservation Start: 2
Reservation End: 12
Reservation ID: 1 is created!
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
1
ROOM INFOS:
Room Type: Single, Daily Cost: 100, Room Size: 15, Has Bath: false
Room Type: Double, Daily Cost: 180, Room Size: 30, Has Bath: false
Room Type: Club, Daily Cost: 250, Room Size: 45, Has Bath: true
Room Type: Family, Daily Cost: 400, Room Size: 50, Has Bath: false
Room Type: Family With View, Daily Cost: 450, Room Size: 50, Has Bath: true
Room Type: Suite, Daily Cost: 650, Room Size: 80, Has Bath: true
Hotel Name: Ramada Bursa
Room Type: Double
Reservation Month: May
Reservation Start: 13
Reservation End: 17
Reservation ID: 2 is created!
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
1
ROOM INFOS:
Room Type: Single, Daily Cost: 100, Room Size: 15, Has Bath: false
Room Type: Double, Daily Cost: 180, Room Size: 30, Has Bath: false
Room Type: Club, Daily Cost: 250, Room Size: 45, Has Bath: true
Room Type: Family, Daily Cost: 400, Room Size: 50, Has Bath: false
Room Type: Family With View, Daily Cost: 450, Room Size: 50, Has Bath: true
Room Type: Suite, Daily Cost: 650, Room Size: 80, Has Bath: true
Hotel Name: Hilton Bomonti
Room Type: Suite
Reservation Month: May
Reservation Start: 2
Reservation End: 19
Reservation ID: 3 is created!
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
4
Please select one of the extra services from below:
1. Laundry Service
2. Spa Service
1
Type the reservation ID to credit this service:
1
How many pieces of clothing?
3
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
4
Please select one of the extra services from below:
1. Laundry Service
2. Spa Service
2
Type the reservation ID to credit this service:
1
How many days?
3
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
4
Please select one of the extra services from below:
1. Laundry Service
2. Spa Service
1
Type the reservation ID to credit this service:
2
How many pieces of clothing?
5
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
7
Name:
Bill
Surname:
Gates
ID:
123
Monthly Payment:
250
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
7
Name:
Steve
Surname:
Jobs
ID:
234
Monthly Payment:
280
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
8
Type:
Water
Amount
210
Month:
April
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
8
Type:
Electricity
Amount
380
Month:
April
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
8
Type:
Water
Amount
330
Month:
May
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
9
Enter Month:
April
For reservation ID: 1, Service type: Room booking, Service Cost: 4000.00
For reservation ID: 1, Service type: Laundry, Service Cost: 60.00
For reservation ID: 1, Service type: Spa, Service Cost: 300.00
Total monthly income: 4360.00
Total monthly bills due: 590.00
Total monthly employee cost: 530.00
End of month balance: 3240.00
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
9
Enter Month:
May
For reservation ID: 2, Service type: Room booking, Service Cost: 720.00
For reservation ID: 2, Service type: Room booking, Service Cost: 11050.00
For reservation ID: 2, Service type: Laundry, Service Cost: 100.00
For reservation ID: 3, Service type: Room booking, Service Cost: 720.00
For reservation ID: 3, Service type: Room booking, Service Cost: 11050.00
For reservation ID: 3, Service type: Laundry, Service Cost: 100.00
Total monthly income: 23740.00
Total monthly bills due: 330.00
Total monthly employee cost: 530.00
End of month balance: 22880.00
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
10
Customer ID: 3, Service Type: Room booking, Cost: 11050.00
Customer ID: 1, Service Type: Room booking, Cost: 4000.00
Customer ID: 2, Service Type: Room booking, Cost: 720.00
Customer ID: 1, Service Type: Spa, Cost: 300.00
Customer ID: 2, Service Type: Laundry, Cost: 100.00
Customer ID: 1, Service Type: Laundry, Cost: 60.00
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
11
Hotel Name: Hilton Bomonti, Customer ID: 3, Service Type: Room booking, Cost:
11050.00
Hotel Name: Hilton Istanbul, Customer ID: 1, Service Type: Room booking,
Cost: 4000.00
Hotel Name: Ramada Bursa, Customer ID: 2, Service Type: Room booking, Cost:
720.00
1. Create new Reservation with Room Type
2. Display all Reservations
3. List the reservations for a specific city
4. Add extra services to a reservation
5. Calculate total cost for each service
6. Display the total cost of every customer
7. Add an employee
8. Add a bill
9. Get monthly balance
10. List all Services sorted based on cost
11. List all Reservations sorted based on hotel names
12. Exit
12
Exiting, Goodbye!



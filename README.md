# Team 6 MIST 4610 Group Project 1

# Team Name: 
39217 Group 6

# Team Members: 

1. David Tran [@dstudent17](https://github.com/dstudent17/4610-Group-Project-1)
2. Nick Kalenik [@NickKalenik](https://github.com/NickKalenik/MIST4610GroupProject1)
3. Minathi Mekala [@minathi11](https://github.com/minathi11/MISTGroupProject1)
4. Ngoc Nguyen [@ngocpn1](https://github.com/ngocpn1/MISTProject1)
5. Anthony Ramage [@anthonyramage](https://github.com/anthonyramage/MIST-4610-Group-Project-1)
6. CJ Tumlin [@CJTumlin](https://github.com/CJTumlin/MIST4610)

## Problem Description:
Our team has been tasked to model and create a relational database for the operations of "Athens Tennis Haven", a tennis club in Athens, Georgia. The club has a complex network of relationships between club members, tennis courts, club staff, tennis equipment, etc. We plan to accurately model these relationships and populate realistic data for each entity and their attributes. With this data, we will create a series of queries to extract meaningful information from the database to make important business decisions for Athens Tennis Haven.
## Data Model:
Data Model Explanation:

Our model works to ensure a good flow to serve the 3 main entities: courts, members, and employees. A club can have multiple courts that can be utilized in different ways. Maintenance Employees can log the times they will service the courts, members can schedule Sessions for the Lessons with their coaches, and they can make reservations on their own. This is all connected to the Courts table that allows the Tennis Club to see all activities going on within those courts. 
Employees belong to different Departments. Maintenance Employees are connected to the courts through Services, and Coaches can make Lessons, which are connected to the courts through Session, with their students. 
The club has many members. They are Billed individually and can be in Teams. Members can also rent out equipment needed to use at the courts. They can make reservations with the courts to practice either by themselves or for their teams, and they can join a Session to get Lessons with their coach. 

<img width="852" alt="UpdatedDataModel" src="https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/ca2dcc0d-4660-4b4f-974b-4c497db45a86">

## Data Dictionary:
![DataDictionaryFinal](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/82f1212d-230e-4d07-949f-4957ba43e45e)

## Queries:

![ComplexityTable](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/39f4eb59-8d0d-41ef-bd29-41869d5e264c)

1. Query 1 lists the amount of “Fulfilled” maintenance requests by court number. It descends from the highest number of “Fulfilled” comments to lowest.
   
![Query1SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/2bb4fe6f-4a72-4a0a-ab1d-128d3f1b88e1)

Query 1 allows managers to see the courts that require the most amount of maintenance. These courts may see the most use from players or patrons watching games, so it may show management that these courts need significant upgrades to lessen the amount of needed maintenance requests.


2. Query 2 lists all tennis club members and the amount of times they have made a court reservation.
   
![Query2SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/d95389d5-bbd5-40b2-bdac-69ad1bf7542f)

Query 2 allows managers to see how active all members are with court reservations. Management could thank the very active members to keep them happy, and they could contact non active members to improve club participation.


3. Query 3 lists each team, their number of members and the total amount of equipment that each team (through its members) has rented
   
![Query3SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/6bebb276-a267-4ac0-85ca-c433a6d80c22)

Query 3 allows managers to see how active each team is, their number of members and how much each team in total is making rentals of equipment. This would be important for management to know if they wanted to check on their team's activities.


4. Query 4 identifies the type of equipment that has been rented most by members, in descending order.
   
![Query4SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/a4745f1d-6d1e-4360-b1a8-eb9f4661808a)

Query 4 allows management to study the usage rates of the equipment they offer for rent. They could decide to purchase more units of equipment that is in high demand, and they could choose to delay further purchases of equipment that rarely gets rented out.


5. Query 5 produces a list of members that have made at least three court reservations but have not taken any lessons. This query also lists out the members contact information, and orders the members by last name alphabetically.
   
![Query5SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/fc26502f-0a98-45dd-8f83-95076a2fca3b)

Query 5 allows management to determine the beginner-level members who like to play a lot of tennis, but may have not taken any lessons yet. This is a business opportunity for the club, as they can reach out to these members to offer them lessons.


6. Query 6 produces the contact information for members who have not rented out any equipment.
   
![Query6SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/d57f76b4-e80a-4689-90d0-b34ff8dd8a3f)

Query 6 allows management to see members that potentially are not active within the club. Contacting them with a reminder that the club offers equipment rentals may encourage them to rent and thus play more tennis.


7. Query 7 produces the average salary for assistant coaches.
   
![Query7SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/cad65589-d0b4-47f9-83cb-365eefcf77f4)

Query 7 allows management to compare the average salary of their assistant coaches to other clubs in the area. If they are experiencing high coach turnover, they are most likely underpaying them. If they are experiencing high operating costs, they may need to decrease their average pay.


8. Query 8 lists out the names of members and what equipment they have rented within the last 5 months
   
![Query8SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/fdb62eea-70a7-49bb-a8dd-4bb7f9cc2749)

Query 8 can be used by management to track rentals within the last 5 months. This can be important for management to track trends and see what equipment has been rented recently.


9. Query 9 lists all of the employees, their departments, and their salaries in descending order by department.
![Query9SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/0f10e7c8-1ad9-4b63-ba77-d8f29885650c)
Query 9 can be used by management to quickly see what all employees in each department are currently being paid. This can help management when trying to decide how much a new-hire should make or whether an employee is due for a raise.


10. Query 10 will display how many rackets the club has.

    
![Query10SS](https://github.com/NickKalenik/MIST4610GroupProject1/assets/148160069/aa4c6c93-ed78-4322-9268-98f2233458dd)


Query 10 can be helpful to management by providing a quick glance at the quantity of rackets in stock. If they need to purchase more or less, this query can assist them.


## Database Information:
Name of database: ns_F2339217Group6

Additional Information: Each query listed above is marked in the database using stored procedures which can be called using the following format: CALL TP_Qx(), where x is the query number.





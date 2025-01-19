## Loan-Management-System-Using-MYSQL-and-Java-GUI

<img src= "https://visitor-badge.laobi.icu/badge?page_id=201851019-iiitv/Loan-Management-System-Using-MYSQL-and-Java-GUI " alt="visitor badge"/> |  ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/201851019-iiitv/Loan-Management-System-Using-MYSQL-and-Java-GUI/master)

# RUN PROCESS:

1)- First, we should connect our Java IDE with JDBC (Java Database Connectivity). Here is the full reference on how to connect JDBC with MySQL: How to connect JDBC with MySQL. https://www.javatpoint.com/example-to-connect-to-the-mysql-database

2)-Create a database named "project."

3)-Create a table called "new_application" in the "project" database.
 -- -----------------------------------------------------------------
create table new_application(
 name varchar(40),
 mob varchar(40),
 addr varchar(40),
 gender varchar(40),
 dob varchar(40),
 amount varchar(40),
 no_of_year varchar(40),
 loan_type varchar(40),
 username varchar(40),
 password varchar(20),
 status varchar(20),
 primary key(username,password)
 
 
);


-------------------------------------------------------------------------------

Connection con=DriverManager.getConnection(
"jdbc:mysql://localhost:3306/project","root","ambesh");

 *where we change root with our username and ambesh with password of our MYSQL .
*In the code we should change this line of code with this

  By default username is already root.

 #  Run ex.java file
OUTPUT :

   
   
   # 1  After running we get 4 buttons:
   
![4_buttons](https://user-images.githubusercontent.com/48892208/85872981-20e1f480-b7ee-11ea-863e-3c8336d6ff7e.png)

# if we click new Customer , first we  get registration form :
![regist](https://user-images.githubusercontent.com/48892208/85873588-f7759880-b7ee-11ea-9643-2f826f587ff3.png)

# after register we can login as exist customer  by using username and password can see all details  and status of application  :
![login](https://user-images.githubusercontent.com/48892208/85874048-aa45f680-b7ef-11ea-8551-372e59cba96d.png)
![details](https://user-images.githubusercontent.com/48892208/85876473-648b2d00-b7f3-11ea-80df-31c780122c5f.png)


# Admin(Bank manager) can login , then after admin have 3 option  and he can update application status as passed, rejected and no action will shw pending application:
![admin](https://user-images.githubusercontent.com/48892208/85874546-6c959d80-b7f0-11ea-9471-0a7212af45ea.png)
![buttonadmin](https://user-images.githubusercontent.com/48892208/85874550-6e5f6100-b7f0-11ea-8510-7fb430608202.png)

# if Admin choose  pending application then he can see all pending applications :
![pending](https://user-images.githubusercontent.com/48892208/85875179-753aa380-b7f1-11ea-92d0-93d7f284a11c.png)

# if Admin choose  passed application then he can see all passed application :
![passed](https://user-images.githubusercontent.com/48892208/85875172-7370e000-b7f1-11ea-920d-936c6e4f67dc.png)

# Admin can also check a specific user  by using his name and dob and can change the status :
 if status is already passed, then admin do not need to change the status 
 if  status is pending Admin can change the status  to passed/rejected 
 if status is change t rejected then application will be deleted from database
 ![dob](https://user-images.githubusercontent.com/48892208/85875485-e5492980-b7f1-11ea-8f83-6c655eb38275.png)
![data](https://user-images.githubusercontent.com/48892208/85875493-e8441a00-b7f1-11ea-8b2f-a4c397f78fa8.png)

* Admin can see all borrower and how much amount is remaining to pay 

# if user login as exist customer and status is passed then he have 3 option :

![3button](https://user-images.githubusercontent.com/48892208/85876193-fba3b500-b7f2-11ea-8295-731c58caa532.png)

a)Pay the installement : I payment is done, then remaning balance will be updated and als printed on screen
b)Calculate the EMI : User can caculae monthly EMI by entering amount,year and the interest rate that is already filled by bank manager.
c)see remaining balance 
 






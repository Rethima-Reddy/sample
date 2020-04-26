# Northwest Library 
An android application which is used for searching and renting books from a library using android mobile.

<h2>App Name:</h2>
<h3>Northwest Library</h3>

<h2>App Logo<h2>
  <img src="https://raw.githubusercontent.com/Rethima-Reddy/sample/master/Images/appLogo.jpeg" />
  
<h2>Team Members:</h2>
 <li> Anil Bomma</li>
 <li> Deepthi Tejaswani Chokka</li>
 <li> Rethimareddy Polam</li>
 <li> Mahender Reddy Surkanti</li>


<h2> Introduction to our Project:</h2>
<p>
  Our B. D. Owens Library is maintaining website for the book tracking. To know where a specific book is located in library, we need to   use that website only. By our project we will create an android application in which we will keep track of all the books in the         library. Admin will add the book name, details and the location where it is kept and the users will search the book by book name or     description and can see in which place the book is located. The users/Student can also view the books from the library and also know     the details like due date and extra charges for late return from our appliation.
</p>
  
<h2>Specifications/Support Version:</h2>
  <p>
    We are using android API version of pixel 3a XL API 28. The size of the layout is 1080*2160 with a density of 400. The complete details of the device we have used in our project is:
    <li>Device Name: Pixel 3a XL API 28</li>
    <li>Android API: 9.0 API 28</li>
    <li>Size: 1080*2160 </li>
  </p>



<h2>Database:</h2>
  <p> Firebase </p>
  <p> 
    We are using a Persistent database named Firebase Fire Store. By using the fire 
    Store in our application, we can store the data in cloud and sync it across all the devices when ever required. We are storing information regarding user details, books information and borrowed books details in our database. By using this we structure the data depending on our requirements. We can query and fetch data easily as per requirements. We can also dynamically get the data whenever we require. The database will grow dynamically depending on the information stored. We are also using firebase authentication for validating and logging the user into the application. 
  </p>
   
   
   
<h2>APK file</h2>
https://github.com/anil-bomma/android-library-app/blob/master/LibraryApk.apk
    
    
    
<h2>Installation Steps</h2>
<p>
  Installation of this app is much more easier with just few steps. The User can download the apk file of the LibraryApplication App. By  clicking on the apk file, It install's the app in your android mobile. Once the App gets installed the user can click on the App icon to  open it. Later on, the user can use the application as per their requirements.
</p>
  
  
  
<h2>Requirements:</h2>
<p>
  <li>Mobile with the Android operating System.  </li>
  <li>Minimum 1 GB RAM.  </li>
  <li>Minimum 8 GB internal storage  </li>
  <li>To run this app we need internet.  </li>
</p>



<h2>User Credentials for testing: </h2>
<p>
  <h3>Login as Admin:</h3>
  <ul>
    <li><b>UserID:</b> s537157@nwmissouri.edu</li>
    <li><b>Password:</b> 123456</li>
  </ul>
  <h3>Login as Librarian/Department admin:</h3>
  <ul>
    <li><b>UserID:</b> s537240@nwmissouri.edu</li>
    <li><b>Password:</b> 123456</li>
  </ul>
  <h3>Login as Student:</h3>
  <ul>
    <li><b>UserID:</b> s536974@nwmissouri.edu</li>
    <li><b>Password:</b> 123456</li>
  </ul>
</p>


<h2>Sources used for our Project:</h2>
<p>
  For Completion of our project we have used many websites. Few of them are listed below.  
  <li> https://developer.android.com/</li>
  <li> https://stackoverflow.com/ </li>
  <li> https://www.youtube.com/watch?v=fGcMLu1GJEc </li>
  <li> https://www.youtube.com/watch?v=tLVz5wmNyrw</li>
</p>


<h2> Sequential flow and detailed description of our project</h2>
<p>
  Our application <b>Northwest Library</b> allows the users to know the location of book they are searching in B.D Owens Lirary. By using our applictaion the user can find the book they require without wasting their time in searching book manually. They can also know weather the book is available in the library or not using our app. They can borrow a book if required and also view the due date to return the book which they have borrowed earlier.
</p>
<ul>
  <li>
    Once the user open the application even before login, they can view the <b>list of books</b> that are available in our library. They can view detailed <b>description of a book</b> by clicking on a particular book they want.
  </li>
  <li>
    By reading the description the user can know wheather they want that book or not. If they want that book they can perform any of the two options persent. They are as follows: 
    <ul>
      <li>
        One is to <b>view the location</b> of the book in the library and 
      </li>
      <li>
        The other is to <b>borrow that book</b> from the library. 
      </li>
    </ul>
  </li>
  <li>
    To do any of the described actions the login to the application is required. If the user has already logged in and 
    <ul>
      <li>
        Clicked on <b>view the location,</b> the user can see the location of book by section and rack ID of that corresponding book. 
      </li>
      <li>
        Clicked on <b>borrow book,</b> the due date to return the book will be shown and an alert box is displayed to <b>confirm the borrow action</b>. Once user confirmed it, the book ID along with used ID will be added to the <b>borrowed books list</b> in database.
      </li>
    </ul>
    If they have not logged in before, the application will redirect them to <b>login activity</b>.
  </li>
  <li>
    If a user is new to the application, they should <b>register</b> with the personal information and then login using mail id and password. <b>(OR)</b> If already registered but had <b>forgot his/her password,</b> they can request for <b>resetting the password</b> and a <b>email</b> will be sent to the user with the instructions for resetting the password. Initially every user is added with role as student which can later be updated as Librarian/Department admin if the admin wants them to be.
  </li>
  <li>
    So according to the user role the view of the application changes. 
    <ul>
      <li>
      If the User role is <b>Student</b>, they can perform actions like <b>viewing the list of books</b> available in the library, <b>look for the location of a particular book</b> in the library, track the list of the <b>books he/she have already borrowed</b> and check their due dates to return.
     </li>
    </ul>
    <ul>
      <li>
         If the User role is <b>Librarian/Depatment Admin</b>, they can perform all the actions done by the user. A part from that, if new books are bought by libary, those book details and the storage location can be <b>added(book) into database</b> by the him/her. They can also view the <b>list of books borrowed by students</b> along with their corresponding #919 number and due date to for every book.
      </li>
    </ul>
    <ul>
      <li>
         If the User role is <b>Admin</b>, he/she can perform all the functionalities done by student and department admin. A part from that, they can also make a student as librarian/department admin by <b>adding them to Department Admin list</b>. This privilage is given only to admin. Admin can also view the <b>list of librarians/department admins</b> present. He/She can <b>remove</b> a person's role from librarian/department admin and make them a normal user that is, Student if they want.
      </li>
    </ul>
    </li>
  <li>
    Apart from all the mentioned functionalities, all users who login are provided with some other basic features like view the <b>user profile, change password, help screen and Contact Us</b> page with all the related data in it.
  </li>
</ul>






<h2>Layouts of our project:</h2>
<h3>Splash Screen:</h3>
<p>
  This is the welcome page to our application. The splash screen will be the launch page of our application. This screen acts as a loading page before launching the application. 
</p>
<img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/SplashScreen.png" width="200" height="400"/>

<h3>List all books:</h3>
<p>
  This is the main activity of our application. This screen consists of list of all available books in the library. The screen appears as below.
</p>
<img src="https://raw.githubusercontent.com/Rethima-Reddy/sample/master/Images/listBooks.png" width="200" height="400" />

<h3>Basic Navigation bar:</h3>
<p>
  This is the navigation bar to any user who didn't log in. Shown are the list of functionalities a user can do before logging into the application.
</p>
<img src="https://raw.githubusercontent.com/Rethima-Reddy/sample/master/Images/new_BasicNavBar.png" />


<ul>
   <h3>Login Screen:</h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/LoginScreen.png" />
  <p>
    The login page will be used for the app in which the user will enter their credentials like username and password of if they are new user they have button called register, by clicking it they will redirect to registration page where the details of the user/students are entered. 
  </p>
</ul>
  <ul>
   <h3>Registration Screen :</h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/RegisterScreen.png" />
  <p>
If the student/user is new to the application they need to register themselves into this by giving the basic details for them like name, #919 number and contact details. We will also add form validations for the inputs given.
  </p>
  </ul>
  <ul>
   <h3>Home Screen:</h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/ListAllBooks.png" />
  <p>
The user will enter into home page of the application. This screen will display the list of books available in our library app. By clicking upon that particular book, you will be re-directed to "About the Book" Screen.  
  </p>
  </ul>
    <ul>
   <h3>About the Book Screen:</h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/AboutTheBook.png" />
  <p>
This screen is useful to know the in-depth information of that particular book. If the user is interested in borrowing the book, the user can click upon the BORROW BOOK Button. The borrow book button allocates the user to borrow a book as and when required. 
  </p>
  </ul>
   <ul>
   <h3>Navigation Screen:</h3>
  <p>
    The functionalities present in this app can be displayed in the navigation screen as displayed below. This navigation screen will be a basic screen which is displayed to the user of the book app.
  </p>
  
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/InitialFragment.PNG" />
  
   <p>
The screen displayed below is the navigation screen which is to be available for the department admin. We are making sure that all of the functionalities which are available are available to only certain people.
  </p>
  
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/LoginAsAdmin.PNG" />
 
  </ul>
  <ul>
   <h3>Book Search Screen : </h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/SplashScreen.png" />
  <p>
This screen will show up search option will be displayed on top of screen and the sections under it. Once the book needed is selected the section and the row in which the book is present is highlighted. 
  </p>
  </ul>
  <ul>
   <h3>Profile Screen:</h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/UserProfile.PNG" />
  <p>
This page will show the details of the user/student which they have entered at the time of registration.
  </p>
  </ul>
  <ul>
   <h3>Adding Books Screen:</h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/AddingABook.PNG" />
  <p>
This privilege is only given to admins. Every time a new book imported, the book details are entered by the admin. This page will contain all the edit text to add details of the book. The details will be stored in database.
  </p>
  </ul>
  
   <ul>
   <h3>Change Password Screen:</h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/ChangePassword.PNG" />
  <p>
    If the person who has logged in desires to change the password, then the concerned person can do so in this page.
  </p>
  </ul>
  
   <ul>
   <h3>Contact-Us Screen:</h3>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/ContactUsScreen.png" />
  <p>
   The contact-us screen is used to display the details to contack in case of occurence of any queries. They can reach out to a person by through email or by calling the concerned person. An individual can re-direct to the concerned option required by clicking upon the displayed buttons. 
  </p>
  <img src="https://raw.githubusercontent.com/anil-bomma/android-library-app/master/Images/ContactUsRedirectScreen.PNG" />
  
  </ul>
  

 

Create Table Book_master ("ISBN" varchar (10) PRIMARY KEY,
"title_of_book" varchar(50) ,"yr_of_publication" INT, "Lang" varchar(50),"Category_type" INT, "Details" Varchar(1000),” book_id” int(5),"No_Of_Copies_Current" INT)
SELECT * FROM book_master
INSERT INTO Book_Master values('S0001','OPERATIONS MANAGEMENT',05,'ENGLISH',3,'This book covers the course material for Management and supply chain',10)
CREATE TABLE Category_Master ("Category_id" INT PRIMARY KEY, "Category_Name" VARCHAR (50), category_place varchar varchar (10))
SELECT * FROM Category_Master
INSERT INTO Category_Master values (2,'Science', 2nd floor’)
CREATE TABLE Borrower_details (Borrower_ID INT, ISBN Varchar (10) ,Borrowed_On_Date datetime , PRIMARY KEY (Borrower_ID, ISBN, Borrowed_On_Date),Borrowed_To_Date datetime, Book_Return_date datetime, Given_by INT)
SELECT * FROM Borrower_details
INSERT INTO Borrower_details VALUES (B1000,'S0001','11/14/2013','12/14/2013','12/15/2013',’Staff089’)
CREATE TABLE staff_master (User_id INT PRIMARY KEY, User_Name VARCHAR (100), user_mail varchar (20), user_phone int (13), role VARCHAR (50))
SELECT * FROM staff_master
INSERT INTO staff_master VALUES (‘Staff089’,'Lewis','lewis@gmail.com',’559-347-9098’,’issue’)
CREATE TABLE Student (Student_id INT PRIMARY KEY,
 Student_Name VARCHAR (50), Sex VARCHAR (6), DOB datetime, student_mail varchar(15) Borrower_ID INT UNIQUE, Course VARCHAR(50), Address VARCHAR(300), Phone  INT UNIQUE
)

SELECT * FROM Student
INSERT INTO Student VALUES (‘St234’,'Christina','Female','17/11/1989',’christina@gmail.com’,'B1000','Science','California',’9791566020’)
CREATE TABLE Videos_Master (
 Video_ID VARCHAR (50) PRIMARY KEY,
 Video_name varchar (100),
 Author VARCHAR (100),
 Duration INT,
Video_category varchar (20),
 Production_date datetime,
 Publisher_name VARCHAR (100)
)
INSERT INTO Videos_Master VALUES ('VD345','javatutorials’,'Balguruswamy','68'','Technology','12/17/2008','Das Publishers')
SELECT * FROM videos_master
CREATE proc GetBooksbyBorrowerID @Borrower_id INT
AS
BEGIN
SELECT Z.BORROWER_ID, x.ISBN, y.book_Title, b.LANGUAGE, Covert (VARCHAR, a.borrowed_from_date,11/14/2013)"Borrowed on (mm/dd/yyyy)" FROM borrower_details a, book_mst b
WHERE z.borrower_id=@Borrower_id
AND x.ISBN = b.ISBN
END
GO
EXEC SP_Task1 12345
SELECT COUNT (*)AS "Total No.OfBooks Borrowed" FROM borrower_details WHERE borrower_id=@Borrower_id AND CONVERT(VARCHAR,borrowed_from_date,11/14/2013) BETWEEN  @on_date AND @to_date
END
GO
EXEC SP_Task2 ‘12345’,'10-11'
ALTER proc GetBooksByCategory @Category_Name VARCHAR (100)
AS
BEGIN
DECLARE @category_id INT
SET @category_id = (SELECT category_id FROM category_master WHERE category_name =  (science(math@Category_Name)))
SELECT a.Category_id, a.Category_Name, SUM (b.no_of_copies_current)"Total No.Of Copies"
FROM Category_Master, a.book_master b WHERE a.Category_id=b.category_type AND a.Category_id = @Category_id GROUP BY a.Category_id, a.Category_Name
END
GO
EXEC Task2 '6789'


<?php include("header.php"); ?>  
<link rel="stylesheet" href="files/template.css" type="text/css"> 
<link rel="stylesheet" href="files/constant.css" type="text/css"> 
<style type="text/css"> 
 .style3
 {
color: #FFFFF
}
 .style10
 {       
  font-size: 10px;        
 color: #101010; 
} 

.style12 
{
margin: 0 0px 8px 0; 
padding: 16px  27px; 
color: blue;
}

 .style20
 {font-size: 14px} 
 </style> 
<div id="content">      
 <div class="clear">     
   
<div class="left-indent">
<div class="clear">    
<div class="border-left">
<div class="border-right">     
<div class="border-top">
<div class="border-down">
<div class="corner-top-right">     
<div class="corner-top-left">
<div class="corner-bottom-left">     
<div class="corner-bottom-right ">        
 <div class="wrapper-box-indent">     
<div class="box-title">    
 <div class="border1-left">    
 <div class="border1-right">    
 <div class="border1-top">     
<div class="border1-bottom">     
<div class="corner1-top-right">    
 <div class="corner1-top-left">     
<div class="corner1-bottom-left">     
<div class="corner1-bottom-right "> 

<h3>Main menu</h3> 
        </div> 
        </div>         
</div>         
</div>        
 </div>         
</div>         
</div>         
</div>         
</div>                                                                              
<div class="main-box">     
<div class="clear">        
 <ul class="menu">                          
<li id="active item1">
 <a href=" ">
<span>Home</span>
</a></li>                        
  <li class="item2">
<a href="">
<span>Get notifications </span>
</a>
</li>                                          
<li class="item29">
<a href="">Register forBooks</a>
</li>                                    
<li class="item30">
<a href="">Brief about book</a>
</li>        
 <li class="item31">
<a href="">
<span>Details of book</span>
</a></li>                    
  <li class="item32">
<a href="">
<span>Search books</span>
</a>
</li>                                          
<li class="item33">
<a href="">
<span>What's New? </span>
</a>
</li>         
</ul>         
</div>     
</div>     
</div>     
</div>         
</div>         
</div>         
</div>         
</div>         
</div>         
</div>         
</div>     
</div>  

 <div class="wrapper-box module s1">         
<div class="border-bottom"> 
<div class="corner-bottom-left">         
 <div class="border-left">         
<div class="border-right">         
<div class="corner-top-left">        
 <div class="corner-top-right">                  
<div class=”border-top”>  
<div class="corner-bottom-right ">  
     
<div class="wrapper-box-indent">         
<div class="box-title">    
 <div class="border1-top">  
<div class="corner1-top-left">        
 <div class="border1-left">         
<div class="border1-right">
<div class="border1-bottom">        
   <div class="corner1-bottom-right ">
   <div class="corner1-top-right">       
  <div class="corner1-bottom-left">         
<h3>Popular</h3>      
</div>         
</div>        
 </div>         
</div>         
</div>         
</div>         
</div>         
</div>         
</div> 

 <div class="main-box">  
 <div class="clear">     
  <ul class="mostread s1">               
  <li class="mostread s1">
<ahref="" class="mostread s1">Book Registration </a>
</li>  
 <li class="mostread s1">
<ahref="" class="mostread s1"> Overview</a>
</li>       
<li class="mostread s1">
<ahref="" class="mostread s1">Extensions of library</a>
</li>
 <li class="mostread s1">
<ahref="" class="mostread s1">What's New in Library?</a>
</li>   
<li class="mostread s1">
<ahref="" class="mostread s1">Welcome to Library!</a>
</li>                 
<li class="mostread s1">
<ahref="" class="mostread s1">Contents of book</a>
</li>        
<li class="mostread s1">
<ahref="//bsahaj" class="mostread s1">Book availability</a>
</li>  
</ul> 
 </div>
 </div>   
      </div>         
</div>         
</div>         
</div>         
</div> 
        </div>
         </div>         
</div>         
</div>         
</div>         
</div>         
</div>         
</div> 

<div id="container" class="wrapper-container"> 
       <div class="corner-top-right">
             <div class="corner-top-top">
<div class="corner-top-right">        
<div class="corner-bottom-right">        
<div class="corner-bottom-left">        
 <form action="chkbookreg3.php" method="post" name="form1">
                  <div>                    
<h2>
<span class="component heading style6">  
                  <span class="style10">
Fill the following book  details:</span>
</span> 
                   </h2>        
          </div>                        
 <p>
</p>            
<table width="290" height="520" border="0" align="center" cellpadding="8" cellspacing="3">             
 <tr>                
<td width="85" align="right" valign="middle" bgcolor="white">  
              <td colspan="2" align="left" bgcolor="black">                 
 <span class="style6">                  
<script type="text/javascript">                                     
var f1 = new LiveValidation('fname');  
f1.add(Validate.Presence,{failureMessage: " Please enter Firstname"});                                    
 f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$/i ,failureMessage:" It takes only characters"}); 
 f1.add(Validate.Format,{pattern: /^[a-zA-Z][a-zA-Z\s]{0,}$/,failureMessage:" Invalid "});                                 
 </script>                  
</span>
</td> 
 </tr>    
          <tr bgcolor="white">  
              <td align="right"  bgcolor="blue">
<p style="color: #000000">From:</p>                 
 <td colspan="3" align="left" bgcolor="white">
<span class="style8 style1">                
  <label>                  
SELECT Z.BORROWER_ID, x.ISBN, y.book_Title, b.LANGUAGE, Covert (VARCHAR, a.borrowed_from_date,11/14/2013)"Borrowed on (mm/dd/yyyy)" FROM borrower_details a, book_mst b
WHERE z.borrower_id=@Borrower_id
<?php }?> 
  <script type="text/javascript">                                          
 //var f1 = new LiveValidation('staff');  
 //f1.add(Validate.Presence,{failureMessage: "Please enter staff name"});                                                                        </script>                
  </select>                  
<script type="text/javascript">                                     
var f1 = new LiveValidation('mname');  
 f1.add(Validate.Presence,{failureMessage: " Please enterMiddlename"}); 
  f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$,failureMessage:" It takes only characters"});

 f1.add(Validate.Format,{pattern: /^[a-zA-Z][a-zA-Z\s]{0,}$/,failureMessage:" Invalid "});   
 </script>  
 </label>    
            </span>
</td>              
</tr>              
<tr>               
 <td height="26" align="left" valign="middle" bgcolor=”white">  
                           
<td align="left" bgcolor="#FFFFFF">
</td> 
             </tr>             
 <tr>                
<td height="30" align="left" valign="middle" bgcolor="white">
<span style="color: “black">Enter Your Message:</span>                
<td width="276" align="left" bgcolor="white">
<label>                 
 <textarea name="address" cols="40" rows="9"  id="address">
</textarea> 
                                
 <script type="text/javascript">   
 var f1 = new LiveValidation('address');   f1.add(Validate.Presence,{failureMessage: " Please enter Address"});                                    
//f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$/i ,failureMessage:                                   
 // " It takes only characters"});  

 //f1.add(Validate.Format,{pattern: /^[a-zA-Z][a-zA-Z\s]{0,}$/,failureMessage:" Invalid Address"});  

                                </script> 
                 </label>               
 </span>
</td> 
</tr>              
<tr bgcolor="#999999">               
 <td align="right" valign="middle" bgcolor="red">               
 <td colspan="3" align="left" bgcolor="black">
<span class="style15 style3">                 
 <label>                  
<script type="text/javascript">                                    
 var f1 = new LiveValidation('contactno'); 
  f1.add(Validate.Presence,{failureMessage: " It cannot be empty"});                                    

 f1.add(Validate.Format,{pattern: /^[0-9]+$/ ,failureMessage: " It takes only numbers"});                                    

 f1.add( Validate.Length, { minimum: 8, maximum: 14 } );                                  
</script> 
                 </label> 
               </span>
</td>             
 </tr>              
<tr bgcolor="#993366">    
  <td align="right" valign="middle" bgcolor="white">                
<td colspan="3" align="left" bgcolor="red">
<script type="text/javascript">                                     
var f1 = new LiveValidation(' campus emailid');                                     
f1.add(Validate.Presence,{failureMessage: " Please enter  campus email-id"});                                     
f1.add( Validate.campusEmail );                                  
</script>                             
 </td>              
</tr>              
<?php /*?>
<tr bgcolor="#FFFFFF">                
<td align="right" valign="middle" bgcolor="white">
<span class="style6">Choose Id-Proof: </span>                             
<td colspan="6" align="left" bgcolor="#FFFF">

<select name="idproof" size="1"  id="idproof" >                  
  <option value="Citizenship card">Citizenship card</option>                    
<option value="College ID">College ID</option>                   
 <option value="License Card">License Card</option>                    
<option value="Fee receipt">Fee receipt</option>                                                                            
 <script type="text/javascript">
   var f1 = new LiveValidation('idproof');    
f1.add(Validate.Presence,{failureMessage: "Please enter identification proof"}); 
 </script>                  
 </select>               
 </span>                        
</td>             
  </tr>              
<tr bgcolor="white">               

<td align="right" valign="middle" bgcolor="white">
<span class="style6">Number of Id-Proof:
</span>                               
 <td colspan="6" align="left" bgcolor="white">
<label>                  
<input type="text" name="idproofno" id="idproofno" maxlength="12">                                 
 <script type="text/javascript">
var f1 = new LiveValidation('idproofno'); 
 f1.add(Validate.Presence,{failureMessage: " It cannot be empty"});                                   

 f1.add(Validate.Format,{pattern: /^[0-9]+$/ ,failureMessage: " It allows only numbers"});                                    

</script> 
                  </label>                               
  </span>
</td>            
  </tr>
<?php */?>            
</table>                   
<p>&nbsp;</p>                     
<input name="submit" type="submit" class="header-button" id="submit" value="Send"/> 
        
</form>            
 </div> 
       </div>
         </div> 
        </div>         
</div>  
     </div>  
   </div>  
</html>
</body>
Save as lib.php

Lib1.reg
<script type="text/javascript" src="jquery.js">
</script> 
<script type="text/javascript"src="ui/jquery.ui.core.js">
</script>         

<script type="text/javascript"src="ui/jquery.ui.widget.js">
</script>        

<script type="text/javascript" src="ui/jquery.ui.datepicker.js">
</script> 
        
<link type="text/css" href="demos.css" rel="stylesheet" />         
<script type="text/javascript" src="ui/jquery.jtimepicker.js">
</script>         
<script type="text/javascript">        
$(function() 
{                          
$('#date').datepicker(
{                        
changeMonth: true,                         
changeYear: true,                        
rangeyear: '2000:2015'                
}); 
               
$('#txtjoin').datepicker
({                         
changeMonth: true,                        
changeYear: true,                
});                      
         
</script>         
<style type="text/css">
  .style3
 {color: #FFFFFF} 

.style6
{       
 font-size: 12px;         
color: #FFFFFF; 
}

.style8
{
margin: 0 0px 5px 0; 
padding: 14px 0 1px 7px; 
color: Black; 
line-height: 40%;
} 

.style10 {
font-size: 12px
}

.style12 
{
margin: 0 0px 10px 0; 
padding: 12px 0 2px 7px; 
color: #FFFFF; 
line-height: 180%; 
font-size: 14px; 
} 


.style20 {font-size: 11%; } 
 
<div id="content">      
<div class="clear">        
          
<div id="left">     
<div class="left-indent">
<div class="clear">     
<div class="wrapper-box module_menu">
<div class="border-left">
<div class="border-bottom">    
<div class="border-top">
<div class="border-right">
<div class="corner-top-left">     
<div class="corner-top-right">
<div class="corner-bottom-right">    
<div class="corner-bottom-left">
    
    <div class="wrapper-box-indent">     
<div class="box-title">    
<div class="border1-left">     
<div class="border1-bottom">     
<div class="border1-left">
<div class="border1-right">
<div class="border1-right">    
<div class="corner1-top-left">    
<div class="corner1-top-right">    
<div class="corner1-bottom-left">     
<div class="corner1-bottom-right">


<h3>Main menu</h3> 
       </div>    
     </div>      
   </div>        
 </div>        
 </div>        
 </div>        
 </div>         
</div> 
       </div>  
  <div class="main-box">   
 <div class="clear">       
 <ul class="menu">                         
<li id="current" class="active item1"> 
<a href=""><span>Home</span></a></li>  
                       
<li class="item2">
<a href=""><span>Get notifications </span></a></li>                                         
<li class="item29">
<a href="">Register for books </a></li>  

 <li class="item30">
<a href=""> Library stand </a>
</li>  

                   <li class="item31">
<a href=""><span>Contact library</span></a></li>   


                                      <li class="item32">
<a href=""><span>Search</span>
</a>
</li>                                          
<li class="item32">
<a href=""><span>What's New? </span></a>
</li>  
      </ul>       
 </div>     </div>     </div>     </div>         </div>         </div>         </div>    </div>         </div>         </div>         </div>     </div> 
        
<div class="wrapper-box module s1">         
<div class="border-left">        
<div class="border-bottom">        
<div class="border-left">         
<div class="border-top">        
<div class="corner-bottom-left">         
<div class="corner-top-right">         
<div class="corner-top-left">        
<div class="corner-bottom-right "> 
      
 <div class="wrapper-box-indent">         
<div class="box-title">     
<div class="border1-top">        
<div class="border1-bottom">         
<div class="border1-left">        
<div class="border1-right">         
<div class="corner1-top-left">         
<div class="corner1-bottom-right">         
<div class="corner1-bottom-left">         
<div class="corner1-top-right ">   
<h3>Popular books</h3>
                 </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div> 
                <div class="main-box">     
   <div class="clear">          
<ul class="mostread s1">             
<li class="mostread s1">
<a href="" class="mostread s1"Contact Numbers</a></li>
  <li class="mostread s1">
<a href="" class="mostread s1"> RegisterBooks</a></li>  
<li class="mostread s1">
<ahref="" class="mostread s1"> Where should I request for book? </a></li> 
<li class="mostread s1">
<ahref="" class="mostread s1">Which section is the book found ?</a></li>
                
<li class="mostread s1">
<ahref="" class="mostread s1"> Recruitement </a></li>

<li class="mostread s1">
<ahref="" class="mostread s1"what to after book is found"?</a></li>  


 <li class="mostread s1">
<ahref="" class="mostread s1"Books find in library?</a>
</li> 
               </ul>    
    </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>         </div>

 <div id="container" class="wrapper-container">
        <div class="corner-top-right">        
<div class="corner-top-left"> 
<div class="corner-top-top">
<div class="corner-top-bottom">       
<div class="corner-bottom-left">        
<div class="corner-bottom-right">        
<form action="chkbookreg1.php" method="post" name="form1"> 
 <div> 
                  <h2>
<span class="componentheading">
<em> Fill the following Book  details:</em>
</span>                    
</span>
</h2>  
               </div>    
                    <p>&nbsp;</p> 
          <table width="770" height="812" align="center" cellpadding="10" cellspacing="5">  
           <tr> 
 <td width="165" align="right" valign="middle" bgcolor="#FFFFFF"> 
                           
<blockquote>                                
<p><span class="style3">FirstName:</span> 
                                 </p>                               
</blockquote>                
<td align="left" bgcolor="#FFFFFF"> 
                <span class="style3">
                 <input name="fname" type="text" id="fname" size="35" >

                                 
<script type="text/javascript">                                     
var f1 = new LiveValidation('fname'); 
f1.add(Validate.Presence,{failureMessage: " Please enter Firstname"}); 
 
f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$/i ,failureMessage:" It allows only characters"});  


f1.add(Validate.Format,{pattern: /^[a-zA-Z][a-zA-Z\s]{0,}$/,failureMessa: " Invalid Firstname"});   

                              </script>  
               </span>
</td>


</tr>  
<tr bgcolor="White">  
<td align="right" valign="middle" bgcolor="#FFFFFF">   
  <blockquote>
  <p>
<span class="style19" style="color: #000000">Middle Name: </span>  
                            
</p>
                              
</blockquote>                
<td align="left" bgcolor=""><span class="style15 style3">  
               <label> 
   <input name="mname" type="text" id="mname" size="35">  
     <script type="text/javascript">                                   
  var f1 = new LiveValidation('mname');   

f1.add(Validate.Presence,{failureMessage: " Please enter Middlename"});   

f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$/i ,failureMessage: " It takes only characters"}); 

f1.add(Validate.Format,{pattern: /^[a-zA-Z][a-zA-Z\s]{0,}$/,failureMessage: " Invalid"});    
                             </script>  
                </label>     
          </span>
</td>              
</tr>              
<tr>                
<td align="right" valign="middle" bgcolor="white">
                             <blockquote>
                               <p>
<span class="style19" style="color: 000000">Last Name:</span>  
                                
</p>                                
</blockquote>               
<td align="left" bgcolor="#FFFFFF">
<span class="style15 style3">                 
<label>                 
<input name="lname" type="text" id="lname" size="55">  
                               <script type="text/javascript"> 
                                    varf1=newLiveValidation('lname');  
   f1.add(Validate.Presence,{failureMessage: " Please enterLastname"});   

  f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$/i ,failureMessage: " It takes only characters"}); 

  f1.add(Validate.Format,{pattern:/^[azAZ][azAZ\s]{0,}$/,failureMessage:"Invalid "});   

</script>   
 </label>               
</span>
</td>             
</tr>             
<tr bgcolor="#FFFFFF">   
 <td height="50" align="right" valign="middle" bgcolor="#FFFFFF">
<span class="style19" style="color: #000000">Gender:</span> 


 <td align="leftbgcolor="#FFFFFF">
<span class="style10 style5"> 
                <label> 
 <input type="radio" name="gender" value="Male" />  Male</label> 
 <label>  
 <input type="radio" name="gender" value="Female" /> 
                Female</label>  
 </span
</td> 
 </tr>            
 <tr bgcolor="#FFFFFF">   
 <td height="30" align="right" valign="middle" bgcolor="white"> 
  <p>
<span class="style19" style="color: black">Date of book issued:</span>
 </p>    
  <td align="left" bgcolor="white">
<span class="style10 style2">  
               <label> 
                
<input type="text" name="date" id="date" readonly="yes" writeonly=”no”>                                  
<script type="text/javascript"> 
 var f1 = new LiveValidation('date'); 

 f1.add(Validate.Presence,{failureMessage: " Please enter date"});   
                                                            </script>   
                </label> 
              </span>
</td>
<br />  
             </tr>       
      <tr bgcolor="#009999">    

          <td height="18" align="right" valign="middle" bgcolor="#000000">   
                          <blockquote>  
                             <p><span class="style7">Time when the book was given:</span>
</p>  
</blockquote>
               <td align="left" bgcolor="#00000"> 
                 <span class="style10 style2">                 
<label>
</label>                 
<input type="text" name="time2" id="time2" /
<?php /*<a href="#" id="time_toggler">Time</a> 
 <div id="time_picker" class="time_picker_div"></div>*/?>   
 </span>
</td>            
 </tr>             
<tr>                
<td height="30" align="right" valign="middle" bgcolor="#FFFFFF"> 
<blockquote>  
                           
 <p>
<span class="style12" style="color: #000300"> Your Address:</span>   
                           </p>   
                            </blockquote>              
 <td align="left" bgcolor="#FFFFFF">
<span class="style12 style1">               
  <label>                  
<script type="text/javascript"> 
  var f1 = new LiveValidation('address');   


 f1.add(Validate.Presence,{failureMessage: " Please enter Address"});  

                                 
//f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$/i ,failureMessage: // " It allows only characters"});     

 //f1.add(Validate.Format,{pattern: /^[a-zA-Z][a-zA-Z\s]{0,}$/,failureMessage:  // " Invalid Address"});  
</script>   
               </label> 
              </span>
<span class="style16 style5">
<textarea name="address" cols="22" rows="2"  id="address">
</textarea> 

              </span>
</td>               
</tr>                            
<tr bgcolor="#666766">               
<td align="right" valign="middle" bgcolor="white">
<span class="style19" style="color: #000000">book:</span>

<?php  $bookQuery = "select *from book_mstr";      
SELECT * FROM book_master
INSERT INTO Book_Master values('S0001','OPERATIONS MANAGEMENT',05,'ENGLISH',3,'This book covers the course material for Management and supply chain',10?> 
                  <?php }?>  
                 <script type="text/javascript">                                     
var f1 = new LiveValidation('city')

f1.add(Validate.Presence,{failureMessage: "Please enter book name"});                                                                   
 </script>  

               </select>   
            </span></td>   
          </tr> 

    
       <tr bgcolor="#FFFFFF">  
 <td align="right" valign="middle" bgcolor="white">


<span class="style19" style="color: #000000">Area Name:</span></td> 
  <td align="left" bgcolor="white">
<span class="style12 style3"> 
                <select name="area" size="1"  id="area" >   


                  <?php }?> 


                  <script type="text/javascript">                                          
 var f1 = new LiveValidation('area');  


f1.add(Validate.Presence,{failureMessage: "Please enter area name"}); 
                                                                  
 </script>                 
 </select>   
            </span>
</td>   
          </tr>  
           <tr bgcolor="#993366">    
   <td align="right" valign="middle" bgcolor="white">                            
  <blockquote>                                
<p>
<span class="style19" style="color: #FFFFF">Pin-code:</span></p>  

                             </blockquote></td>   

            <td align="left" bgcolor="white">
<span class="style15 style3">  

   <input name="pincode" type="text" id="ISBN"maxlength="6">                                  
<script type="text/javascript"> 
 var f1 = new LiveValidation('ISBN');  


f1.add(Validate.Presence,{failureMessage: " It cannot be empty"});   


 f1.add(Validate.Format,{pattern: /^[0-9]+$/ ,failureMessage: " It allows only numbers"});                                  
</script>                                
 </span>
</td>
             </tr> 
            <tr bgcolor="#000999">  
             <td align="right" valign="middle" bgcolor="#000000">
                             <blockquote> 
                              <p>
<span class="style9" style="color: #white">Contact number: </span>
                            </p>  
                             </blockquote>
               <td align="left" bgcolor="#	000786	">
<span class="style15 style3">                  
<label>                  
<input type="text" name="contactno" id="contactno" maxlength="18"> 
                                <script type="text/javascript">                                     var f1 = new LiveValidation('contactno');  


f1.add(Validate.Presence,{failureMessage: " It cannot be empty"});                                   


f1.add(Validate.Format,{pattern: /^[0-9]+$/ ,failureMessage: " It allows only numbers"});         

f1.add( Validate.Length, { minimum: 6, maximum: 12 } );                                  </script>  
               </label>                
</span>
</td>              
</tr>             
<tr bgcolor="#993366"> 
  <td align="right" valign="middle" bgcolor="#FFFFFF"> 
                             <blockquote>      
                         <p>
<span class="style19" style="color: #000000">Email-id:</span>   
                        </p>     
                          </blockquote> 
              <td align="left" bgcolor="#FFFFFF">
<span class="style15 style3">                  
<label>                
 <input name="emailid" type="text" id="emailid" size="35" maxlength="254" />    
  <script type="text/javascript">                                    
 var f1 = new LiveValidation('emailid');  

f1.add(Validate.Presence,{failureMessage: " Please enter email-id"});                                

f1.add( Validate.Email ); 
                                </script>  
                </label>                
</span>
</td>          
   </tr>              
<tr bgcolor="#999999"> 
<td align="right" valign="middle" bgcolor="#FFFFFF">
<span class="style3">Book Type: </span>                             
<td align="left" bgcolor="#FFFFFF">
<span class="style15 style3">                  
<select name="booktype" size="1"  id="booktype" >                                 


<option>----select----</option>
<?php  $booktypeQuery 
{                                                   ?>  
    <option value="<?php echo $rowbooktype['book_id']?>"><?php SELECT * FROM book_master
INSERT INTO Book_Master values('S0001','OPERATIONS MANAGEMENT',05,'ENGLISH',3,'This book covers the course material for Management and supply chain',10)?>
</option>                    
<?php }?>   

                <script type="text/javascript">                                    
 var f1 = new LiveValidation('booktype'); 


  f1.add(Validate.Presence,{failureMessage: "Please enter type of book"}); 
                                                              </script>
                 </select>               
</span></td>                
</tr>              
<tr bgcolor="#999999">   
 <td align="right" valign="middle" bgcolor="#FFFFFF">
<blockquote>
                 <p>
<span class="style3">Book Publisher ID:</span>  
             </p>                
</blockquote> 

              <td align="left" bgcolor="">
<script type="text/javascript">  
 var f1 = new LiveValidation('booklocation');  
     f1.add(Validate.Presence,{failureMessage: " Please enter book location"});  


//f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$/i ,failureMessage:                                   
// " It allows only characters"}); 
                                  

//f1.add(Validate.Format,{pattern: /^[a-zA-Z][a-zA-Z\s]{0,}$/,failureMessage:                                                
 //" Invalid Address"});                                 


</script>                         
<textarea name="booklocation" cols="22" rows="3"  id="booklocation"></textarea></td>  


             </tr>              


<tr bgcolor="000999">                

<td align="right" valign="middle" bgcolor="white"><blockquote>


                 <p>
<span class="style3">Choose Id-Proof:</span>               
  </p>              


 </blockquote>                
<td align="left" bgcolor="#FFFFFF">
<span class="style12style1">                 
<select name="idproof" size="1"  id="idproof" >  


 <option value="College ID">College ID Card</option>           
         <option value="Fee receipt">Fee receipt Card</option>       
             <option value="License Card">License Card</option>               
     <option value="Citizenship card" ">Citizenship card</option>  



              <script type="text/javascript">   
                                 varf1=newLiveValidation('idproof');   
                                  f1.add(Validate.Presence,{failureMessage: "Please enter identification proof"});                                                                 
</script>                  
 </select>
               </span>
</td>    
           </tr>  
           <tr bgcolor=""> 
              <td align="right" valign="middle" bgcolor="#FFFFFF">
<blockquote> 
                <p><span class="style9">Number of Id-Proof:</span> 
               </p>   
            </blockquote>   
            <td align="left" bgcolor="#FFFFFF">
<label>                
<input type="text" name="idproofno" id="idproofno" maxlength="12">  
                               <script type="text/javascript">    
                                var f1 = new LiveValidation('idproofno');                                  


 f1.add(Validate.Presence,{failureMessage: " It cannot be empty"});                                  

 f1.add(Validate.Format,{pattern: /^[0-9]+$/ ,failureMessage: " It allows only numbers"});                                   
 f1.add( Validate.Length, { minimum: 6, maximum: 12 } );                                 
 </script>  

             </label>
</td>   
          </tr>      
       <tr bgcolor="#999999"> 


<td align="right" valign="middle" bgcolor="000987">
<blockquote>  
 <p><span class="style3">Brief description of book:</span>  
              </p>            
   </blockquote>               
<td align="left" bgcolor="#FFFFFF">                           
 <textarea name="bookdesc" cols="32" rows="3"  id="bookdesc">
</textarea>     
                      <script type="text/javascript">                                    
 var f1 = new LiveValidation('bookdesc'); 


f1.add(Validate.Presence,{failureMessage: " Please enter book description"});  
//f1.add(Validate.Format,{pattern: /^[a-zA-Z\s]+$/i ,failureMessage:                                   
// " It allows only characters"});  


//f1.add(Validate.Format,{pattern: /^[a-zA-Z][a-zA-Z\s]{0,}$/,failureMessage:                                           
 //     " Invalid Address"}); 
                                
</script>                         
</td>             
</tr>              
<tr bgcolor="">               
<td height="18" align="right" valign="middle" bgcolor="black">

<td align="left" bgcolor="#FFFFFF">&nbsp;
</td>              
</tr>              
<tr bgcolor="">                
<td height="32" align="right" valign="middle" bgcolor="black"> 

                            <blockquote>                                <p>
<span class="style9" style="color: 000000">Photo of book:</span>                             
</p>                                
</blockquote>                
<td align="left" bgcolor="#FFFFFF">
<input name="photo1" type="file" id="photo1" size="45" /></td> 


            </tr>              
<tr bgcolor="">                
<td height="32" align="right" valign="middle" bgcolor="#FFFFFF">                              
<blockquote>                                
<p>
<span class="style29" style="color: 000000">Photo of book:</span> 
                           </p>     
                          </blockquote>                
<td align="left" bgcolor="000123">
<span class="style12 style4">                  
<label>                  
<input name="photo2" type="file" id="photo2" size="45">                  
</label>
</span>
</td> 
            </tr>           
</table>                 
 <p>&nbsp;</p>   
<input name="reset" type="reset" class="header-button" value="Reset" />
<input name="next" type="submit" class="header-button" id="next" value="Next"/> 
                    <p>&nbsp;</p> 
       </form>             
</div>      
 </div>        
</div>         
</div>         
</div>       
</div>     
</div>     
</body>
</html>

</td>               
<td align="left" bgcolor="#FFFFFF">

<select name="book" size="5"  id="book" >                                 
  <option >----select----</option>


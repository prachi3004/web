# web
<!DOCTYPE html>
<html lang="en">
    <head>
        <!-- Latest compiled and minified CSS -->
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
        <!-- jQuery library -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
        <!-- Latest compiled and minified JavaScript -->
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js">
            
        </script>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="description" content="">
        <meta name="author" content="">
        <title>New page</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div>
            <div class="panel panel-primary">
                <div class="panel-heading">FORM</div>
                <div class="panel-body">
                    <form>
                        Full Name: 
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="full_name" maxlength="30">
                        </div>
                        Father's Name
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="f_name">
                        </div>
                        Mother's Name
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="m_name">
                        </div>
                        Roll Number:
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="rollno">
                        </div>
                        Date Of Bith:
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="dob">
                        </div>
                        University Name:
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="uni">
                        </div>
                        Course Name
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="course">
                        </div>
                        Center Code:
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="center_code">
                        </div>
                        Paper Code:
                        <div class="form-group"> 
                            <input type="text" class="form-control" name="p_code">
                        </div>
                        <div class="btn btn-primary" onclick="add()"> submit</div>
                    </form>
                </div>
            </div>             
        </div>     
        
        <script>
            function add()
            {   
                var numbers = /^[0-9]+$/;
                var alpha = /^[A-Za-z]+$/;
     		var flag='t‘ ;
		var minlength=8, maxlength=10;
                
                if(full_name.value.length==0) 
		{
		alert("dont leave name blank");
		flag='f';
		}
                if(f_name.value.length==0) 
		{
		alert("Please Enter fathers name");
               
		flag='f';
		}
                 if(m_name.value.length==0) 
		{
		alert("Please Enter mother's name");
               
		flag='f';
		}  
                
                if(uni.value.length==0) 
		{
		alert("dont leave university name blank");
		flag='f';
		}
                
                if(course.value.length==0) 
		{
		alert("dont leave course name blank");
		flag='f';
		}0
                
                
        
                 if(rollno.value.length==0) 
		{
		alert("Please Enter roll number");
               
		flag='f';
		}
                 if(!(rollno.value.match(numbers)))
                 {
                         alert('Please input numeric characters only');
                  }

                     
                     
                     
                if(center_code.value.length==0)
               
                    { 
                        alert("dont leave center code blank");
                        flag='f';
                    }
	        else    
	         { 
	             if(center_code.value.length > maxlength)
                         {  	        
		         alert("Maximum character limit for center code is 10");  
		         flag='f';		
                           } 
	            if(!(center_code.value.match(number))) 
	             {	
		       alert("Plz enter numeric value only in center code");
		       flag='f';
	            }
	         }
                 
                 
                  if(p_code.value.length==0)
               
                    { 
                        alert("dont leave paper code blank");
                        flag='f';
                    }
	        else    
	         { 
	             if(p_code.value.length > maxlength)
                         {  	        
		         alert("Maximum character limit for paper code is 10");  
		         flag='f';		
                           } 
	            if(!(p_code.value.match(number))) 
	             {	
		       alert("Plz enter numeric value only in paper code");
		       flag='f';
	            }
	         }

                

        
        
        if(flag=='t')
	          {
		        alert("Form accepted");
	             }

                



            }
        </script>
    </body>
</html>

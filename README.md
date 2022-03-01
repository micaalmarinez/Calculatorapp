<html> 

   <head > 

      <script> 

         //function that display value 

         function dis(val) 

         { 

             document.getElementById("result").value+=val 

         } 

           

         //function that evaluates the digit and return result 

         function solve() 

         { 

             let x = document.getElementById("result").value 

             let y = eval(x) 

             document.getElementById("result").value = y 

         } 

           

         //function that clear the display 

         function clr() 

         { 

             document.getElementById("result").value = "" 

         } 

      </script> 

      <!-- for styling -->

      <style> 
         .title{ 

         margin-bottom: 10px; 

         text-align:center; 
         font-size: calc(10px + 1vw);
         width: 630px; 
         height: 40px;

         color:rgb(1, 18, 44); 

         border: solid rgb(0, 0, 0) 3px; 
         background-color:powderblue

         } 

  

         input[type="button"] 

         { 

         background-color:lightblue; 

         color: rgb(0, 0, 0); 

         border: solid black 2px; 
         font-size: calc(8px + 1vw);

         width: 150px;
         height: 100px
         

         } 

  

         input[type="text"] 

         { 

         background-color:white; 
         font-size: calc(8px + 1vw);

         border: solid black 2px; 

         width: 460px;
         height: 100px
         

         } 

      </style> 

   </head> 

   <!-- create table -->

   <body  > 
      

      <div class = title >CALCULATOR</div> 

       


      <table border="4" bordercolor = "black" width="550" height="350"> 

         <tr>
            <td colspan="3"><input type="text" id="result"/></td> 

            <!-- clr() function will call clr to clear all value -->

            <td><input type="button" value="c" onclick="clr()"/> </td> 

         </tr> 

         <tr> 

            <!-- create button and assign value to each button -->

            <!-- dis("1") will call function dis to display value -->

            <td><input type="button" value="1" onclick="dis('1')"/> </td> 

            <td><input type="button" value="2" onclick="dis('2')"/> </td> 

            <td><input type="button" value="3" onclick="dis('3')"/> </td> 

            <td><input type="button" value="/" onclick="dis('/')"/> </td> 

         </tr> 

         <tr> 

            <td><input type="button" value="4" onclick="dis('4')"/> </td> 

            <td><input type="button" value="5" onclick="dis('5')"/> </td> 

            <td><input type="button" value="6" onclick="dis('6')"/> </td> 

            <td><input type="button" value="-" onclick="dis('-')"/> </td> 

         </tr> 

         <tr> 

            <td><input type="button" value="7" onclick="dis('7')"/> </td> 

            <td><input type="button" value="8" onclick="dis('8')"/> </td> 

            <td><input type="button" value="9" onclick="dis('9')"/> </td> 

            <td><input type="button" value="+" onclick="dis('+')"/> </td> 

         </tr> 

         <tr> 

            <td><input type="button" value="." onclick="dis('.')"/> </td> 

            <td><input type="button" value="0" onclick="dis('0')"/> </td> 

            <!-- solve function call function solve to evaluate value -->

            <td><input type="button" value="=" onclick="solve()"/> </td> 

            <td><input type="button" value="x" onclick="dis('*')"/> </td> 

         </tr> 

      </table> 

   </body> 

</html>

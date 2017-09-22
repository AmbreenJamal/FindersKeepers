<h2>Finders Keepers</h2>

<p>Create a function that looks through an array (first argument) and returns the first element in the array that passes a truth test (second argument).</p>
<ul>  
<li>findElement([1, 3, 5, 8, 9, 10], function(num) { return num % 2 === 0; }) should return 8.</li>  
<li>findElement([1, 3, 5, 9], function(num) { return num % 2 === 0; }) should return undefined.<li>  
</ul>
</p><br/>
<p>======================================================</p>  
   
function findElement(arr, func) {  
  var val = 0;  
  for (var i=0; i<arr.length; i++)  
    {  
      if(func(arr[i]))  
        {  
          val=arr[i];  
          return val;  
        }  
  
    } 
  return undefined; 
}     	
  
findElement([1, 3, 5, 8, 9], function(num){ return num % 2 === 0; });	
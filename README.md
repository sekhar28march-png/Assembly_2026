<!DOCTYPE html> 
<html lang="bn"> 
<head> 
  <meta charset="UTF-8"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>রাজনৈতিক সমীক্ষা</title> 
 
<style> 
      h2 { 
       font-size: 15px;   
       color: white; 
       font-size: 18px; 
       text-align: center; 
       font-weight: bold; 
       font-style: normal; 
        } 
 
      h1, h2 { 
      margin: 0.5px 0; /* Adjusts top and bottom margins to 5px */ 
    } 
     
     .question { 
        border: 1px solid aliceblue; 
        padding: 15px; 
        margin: 10px 0; 
        border-radius: 30px; 
    } 
        .question label { 
            margin-right: 15px; 
    } 
 
    label { 
      color:aliceblue 
       
    }   

    /*.form-group {*/
      /*text-align: left;*/       /* label + input aligned left */
      /*margin: 10px auto;       /* keep spacing */
      /*width: 90%;             /* adjust width */
      /*max-width: 400px;       /* prevent stretching too wide */
      /*font-size:15px;*/

    /*}*/

     
    body { 
      background-color:#000000; 
      font-weight: normal; 
      padding: 8px; 
      font-family: Arial, sans-serif; 
      /*text-align: center;*/
      
      
    } 
  
    h1 { 
      color:#12BCDE; 
      font-size: 22px; 
      text-align: center; 
      font-weight: bolder; 
    } 
 
     
    label { 
      margin-right: 8px; 
      font-weight: bold; 
      text-align: center;
    } 
 
    p { 
      color:#FF6F00; 
      font-weight: bold; 
      /*line-height: 1.0;*/
      /* border: 1px solid; 
      border-radius: 10px; 
      border-color: antiquewhite; */ 
    } 
 
    .bold-label { 
    font-weight: bold; 
    text-align: center;
} 
 
      .radio-group { 
      row-gap: 5px; 
      margin-bottom: 15px; 
      border: 2px solid; 
      border-radius: 25px; 
    }  
 
   input[type="text"] { 
      background-color:#000000; 
      color: #FDFEFE; 
      padding: 15px; 
      border: 1px solid #ccc; 
      border-radius: 5px; 
      box-sizing: border-box; 
   }  
 
 
 
 
    input[type="submit"] { 
      width: 350px; 
      height: 50px; 
      background-color: #0033FF;   /* hwb(204 2% 25% / 0.773);  */ 
      color: white; 
      font-weight: normal; 
      font-size: 15px; 
      border-radius: 8px; 
      border: none; 
      cursor: pointer; 
    } 
    input[type="submit"]:hover { 
      background-color: #0099FF; 
    } 
 
    /*input[type="text"] { 
      padding: 15px; 
      border: 1px solid #ccc; 
      border-radius: 5px; 
      box-sizing: border-box; 
    } */ 
 
    input[type="tel"] { 
      background-color: #000000; 
      color:#FDFEFE; 
      padding: 10px; 
      height:20px; 
      border: 1px solid #ccc; 
      border-radius: 5px; 
      box-sizing: border-box; 
    } 
 
    input::placeholder, textarea::placeholder { 
      font-size: 15px;  
      font-weight: bold; 
      color: #CFD8DC;  
      opacity: 0.6;  
    } 
   
.success-message { 
  display: none; 
  color:green; 
  margin-top:10px; 
  font-weight:bold; 
  font-size:1.5em; 
} 
 
.submitting { 
  display: none; 
  color: blue; 
  font-weight: bold; 
  margin-top: 10px; 
} 
 
 
 
iframe#hidden_iframe { display:none; } 
 
  /* ---- THANK YOU overlay (centered) ---- */ 
  .thank-overlay { 
    position: fixed; 
    inset: 0; 
    display: none;           /* shown only after submission */ 
    align-items: center; 
    justify-content: center; 
    background: rgba(0,0,0,0.45); 
    z-index: 9999; 
    border: 2px solid green; 
    /*border-radius: 8px; */
  } 
  .thank-card { 
    width: 92%; 
    max-width: 420px; 
    /*background: linear-gradient(180deg,#003b6b,#002a4e);*/
    padding: 22px; 
    text-align: center; 
    /*box-shadow: 0 12px 40px rgba(0,0,0,0.6);*/ 
    color:#FFFFFF; 
    animation: popIn .28s ease; 
    border: 2px solid green; 
    border-radius: 6px; 
  } 
  .thank-text { font-size:20px; font-weight:800; margin-bottom:18px; } 
 
  .reset-btn { 
    display:inline-block; 
    background:#CCFFFF;  
    color:#00254f;  
    border:none;  
    padding:10px 18px; 
    border-radius:35px;  
    font-weight:normal;  
    font-size:15px;  
    cursor:pointer;  
    height:50px; 
    /*box-shadow: 0 6px 14px rgba(0,0,0,0.3); 
    transition: transform .12s;*/ 
  } 
   
#resetBtn { 
  margin-right: 30px; 
} 
 
 
 
  .close-btn { 
    display:inline-block; 
    background:#CCFFFF;  
    color:#00254f;  
    border:none;  
    padding:10px 18px; 
    border-radius:35px;  
    font-weight:normal;  
    font-size:15px;  
    cursor:pointer;  
    height:50px; 
    /*box-shadow: 0 6px 14px rgba(0,0,0,0.3); 
    transition: transform .12s;*/ 
  } 
   
   
   
   
   
  /*.reset-btn:active { transform:translateY(1px); } 
 
  @keyframes popIn { from { transform: scale(.98); opacity:0 } to { transform:scale(1); opacity:1 } } 
 
  /* responsive tweaks */ 
  /*@media (max-width:768px) { 
    .page-title { font-size:22px; margin-top:8px; } 
    .thank-text { font-size:18px; } 
  } 
  @media (max-width:420px) { 
    .panel { padding:14px; } 
    .thank-card { padding:16px; } 
    .thank-text { font-size:17px; } 
  }*/ 
 
      
  </style> 
</head> 
 
<body> 
  <h1>রাজনৈতিক সমীক্ষা</h1> 
  <h2>আপনার মতামত</h2><br> 
 
  <div class="form-container"> 
    <div class="panel"> 
      <form id="SurveyForm" 
        action="https://script.google.com/macros/s/AKfycbxCva5mQIn_xCezc0GnU3-GoCxenQZjps4gd-sBpONS7mf4TfYK6q6UX9g-Af-_SX7tAQ/exec"  
        method="post" 
        target="hidden_iframe"> 
 
    <label for="Assembly">Assembly Name:</label> 
    <select id="Assembly" name="Assembly" required style="background-color: #000000; width:205px; height: 40px; font-weight: bold; font-size:15px; color:#FFFFFF"> 
      <option value="">Select from the List</option> 
      <option value="109 Khardah">109 Khardah</option> 
      <option value="110 North Dumdum">110 North Dumdum</option> 
      <option value="111 Panihati">111 Panihati</option> 
      <option value="112 Kamarhati">112 Kamarhati</option> 
      <option value="113 Baranagar">113 Baranagar</option> 
      <option value="114 DumDum">114 DumDum</option> 
      <option value="117 Rajarhat Gopalpur">117 Rajarhat Gopalpur</option> 
    </select><br><br> 
    
     
  <label for="Mondal">Mondal Name</label> 
    <select id="Mondal" name="Mondal" required style="background-color: #000000; width:226px; height: 40px; font-weight: bold; font-size:15px; color:#FFFFFF"> 
      <option value="">Select from the List</option> 
      <option value="Mondal - 1">Mondal - 1</option> 
      <option value="Mondal - 2">Mondal - 2</option>
      <option value="Mondal - 3">Mondal - 3</option>
      <option value="Mondal - 4">Mondal - 4</option>
  </select> <br><br>




    <label for="Ward">Ward Number</label> 
    <input type="text" id="Ward" name="Ward" placeholder="Enter Ward Number" required style="width:226px; height: 40px; font-size:20px; font-weight: bold;"> 
    <br><br>
     
 
    <label for="Booth">Booth Number</label> 
    <input type="text" id="Booth" name="Booth" placeholder="Enter Booth Number"required style="width:222px; height: 40px; font-size:20px; font-weight: bold;"> 
    <br><br> 
 
 
  <div class="question"> 
    <p>Q1. পশ্চিমবঙ্গে বর্তমান সরকারের দুর্নীতির কারণে শিক্ষা, স্বাস্থ্য, খাদ্য ব্যবস্থা ভেঙে পড়েছে</p> 
      <input type="radio" id="q1_yes" name="q1" value="হ্যাঁ" required> 
      <label for="q1_yes">হ্যাঁ</label> 
 
      <input type="radio" id="q1_no" name="q1" value="না"> 
      <label for="q1_no">না</label> 
 
      <input type="radio" id="q1_dk" name="q1" value="জানিনা"> 
      <label for="q1_dk">জানিনা</label> 
  </div> 
       
  <div class="question">  
    <p>Q2. আরজিকর কাণ্ডে পশ্চিমবঙ্গ সরকার তথ্য প্রমাণ লোপাট করেছে</p> 
      <input type="radio" id="q2_yes" name="q2" value="হ্যাঁ" required> 
      <label for="q2_yes">হ্যাঁ</label> 
 
      <input type="radio" id="q2_no" name="q2" value="না"> 
      <label for="q2_no">না</label> 
 
      <input type="radio" id="q2_dk" name="q2" value="জানিনা"> 
      <label for="q2_dk">জানিনা</label> 
  </div> 
 
  <div class="question"> 
    <p>Q3. বর্তমান সরকারের অধীনে হিন্দু সম্প্রদায় পশ্চিমবঙ্গের বিভিন্ন জেলায় অত্যাচারিত</p> 
      <input type="radio" id="q3_yes" name="q3" value="হ্যাঁ" required> 
      <label for="q3_yes">হ্যাঁ</label> 
 
      <input type="radio" id="q3_no" name="q3" value="না"> 
      <label for="q3_no">না</label> 
 
      <input type="radio" id="q3_dk" name="q3" value="জানিনা"> 
      <label for="q3_dk">জানিনা</label> 
  </div> 
 
  <div class="question"> 
    <p>Q4. আগামী বিধানসভা নির্বাচনে বিজেপিকে পশ্চিমবঙ্গে একটা সুযোগ দেওয়া উচিত</p> 
      <input type="radio" id="q4_yes" name="q4" value="হ্যাঁ" required> 
      <label for="q4_yes">হ্যাঁ</label> 
 
      <input type="radio" id="q4_no" name="q4" value="না"> 
      <label for="q4_no">না</label> 
 
      <input type="radio" id="q4_dk" name="q4" value="জানিনা"> 
      <label for="q4_dk">জানিনা</label> 
  </div><br> 
 
  <label for="Phone">Phone Number:</label> 
    <input type="tel" id="Phone" name="Phone"   
           style="height:50px; width:220px; font-size:25px; font-weight: bold; padding:15px" 
           inputmode="numeric" pattern="[0-9]{10}" required 
           placeholder="Enter 10-Digit Ph.Number"> 
           <br><br> 
           <p id="phoneMessage" style="display:none; font-weight:bold; font-size:14px;"></p> 
           
  <input type="submit" value="Submit"><br> 
   
  <P style="color:#33FF00;  
    font-size:15px; font-weight: normal; text-align:center"> আপনার মতামত সম্পূর্ণ নিরাপদ</P>
  <P style="color:#33FF00;  
    font-size:15px; font-weight: normal; text-align:center"> Developed by: Sekhar Sengupta</p> 
  </form> 
  </div> 
  </div> 
     
  <!-- hidden iframe receives the POST response --> 
  <iframe name="hidden_iframe" id="hidden_iframe"></iframe> 
<!-- Thank-you overlay (centered). Reset button below message. --> 
  <div class="thank-overlay" id="thankOverlay" role="dialog" aria-hidden="true"> 
    <div class="thank-card" role="document"> 
      <top><image src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAOEAAADhCAMAAAAJbSJIAAAAmVBMVEUAgAD////l5eUAdgAAeAD4+Pju7u77+/vq6urj4+P1+vXx8fH19fUAcwAAegDk6eTR4tHe497l6uWdwp1Nl03v9O9IlUjr8OuLuIvz7/MriCtQllBpnmn9+f2Yu5hrpGu20La0yLTL2ct6q3p3rXfF2cWPs4+ux64zjDPP3s+80rxjnWM+jz7X4NejwqNcmlwYfxiOuI6cvJwGkbl4AAAIyklEQVR4nO2d63baOBSFkW18t9KmpdQQCENoSUKTXt7/4UY2Actgy5Kse7J/jNaclQz6RtI58kZWJgCAqed5U9SiJkRNiFqOaM4XzUjRqInGvNHJOyVMhEVpCUWw9BBOp9M8DMMctajJUJOh1qHo5OJ/e+Il1WAk3AMX0USzoWh7MAjRZDCKEbaXWYx+JJ3f3NykaTpDzQy1qJmjRnf0tommxygow7hvyveMYbhdHxbQ9/0g8Cud/on/m+yo3xPt+Bm4OKy3fWN4PYPz1dM9DODELqEe3z+too51eL2gnh993d3lVPH4RFEtZktb+SoVy7TsImwS6GpjM18lf18eCZO3JXmRaXaF7h6OVrGrMk3SUy3uAt39E6DgDvRUCw/c2ZZAuwXvSpywSa6rnQsjWAnuVk35wzLNxv41eFKxaYp/Uy1m7gCijDrrqBZL3b0SquXqPIanrdqz7YWwLf95dVqHb7l09ai7T4L19bJaPLk1hCjZfGoIk4rwXnePRAs+nAiPmSZ2o9bjgiFeLeKtK8W+UbDFn57itYNjuI4xry0/6O6PBB1K3Gtb6O6OBC1a1cK9SYqmKYgbwtS1aljJTzGvbe5eKkXJdI55bTdOEt5g1eLWdcLE4TFM3kGmcZnQ/WoRN17bzEnCWVh9O+N8tUjeSbVwewxdXodZ47U5nUvfA2HiLGHjtbmdaT6qhb06Ebr/jO9yLv14erJdH16b/frw2uyXnV4bhIEfQLpvWSysFrD49Xfz8vKyef1dUEBaVy2gv56Bs/aLwYVlm9dW7CLQ0usQomVeW/EDXGq+IE9Vu56e4MsVIBL5lJNVT0/BbRcgiP4Qf8kiry3oHEGkG9J5Sou8tl5AAL4TlqI91YIACABheVnjtRUkQNIg2uK1VWcMCbrtX4mWPFsMAJJOAtlRLQYBwe/e37XCaxsGBD97B9EGr40CEPzrJbTg6YkGEHwhEJpeD6kACbP0NIZ5bug6pAMkZZp5zWZsLqUEpK0W5tVDWsA5XcU3z2ujBQR/h8bQUK+NGpB0uNnkXEoP+GonIT0g8Y1C3GuLjHrGpwckv2JgrNfGAPiVaLaZ6rUJAzT16UkcoKFem0BAM702kYBGVguhgCZ6bWIBDfTaGAC/0XxHatyzhWhA46qFcEDTvDbxgIZ5bYKTTC2jvDYZgEbVQ18GIOa15brXoRzA2mvLjfDaJAGaUw9lARrjtUkDNMVrk5JFjzIjl0oo9GcZQSgT0AivTeIUnVSEldcW6cw0cgEN8NokA+p/epINqN1rk1cHz59Qe225rlwqH5CvWsBKfJ938enyATkIg+Drzy9f1g+/itGrVgUgs9dW3J/PIUfP38bdkyk9ydRie7bwl/PWBz8NnLEmSupOphFTtSg2V5/9wD2MigCZvLbOZbPnRFQFePTaplReW0+f/uNCVLMGK9F7bf5rTw94ENUBMlSL3719YEdUCNjy2jLSOizm/b1gRVRSB0+i9tr6hxCwphulgNT1MLh+4QjXKwOiWkBqr60Y6Ms/akTFgNRe23KoN7SjqDLJ1KLMpdWFwwP6ToWoHJCa8N9wj2gQle1krgkHvDbYV+7ZEDUA0nptNGOIEAeeL9VP0Qm913ZP1S8yohZA6qenX3Q9IyHqATyPYYaUE7y2YjoWURNg5bVVbIP1EO4pe9eHqAuQ/tnikbZ/3YjaAOkJO96EZ0DUB9j22ohOFKTu4zWiRkAGrw3SFYwuRB2FvpuQ7LX5XzgRiyeNgJjXFg16bQUfol7A2muLpjGdq8+FWGy1AjKea+NAZAAUnmTeCJm+mWFG1A5I77XxIeoHfPPaMvpvuZkQ6bcJ0gA5zrUxID486wfkOdfGgGgAINe5NvGIEgH5vscXjSgTkPNcm1hEKYX+ijAMY5ZzbSIR5QJyn2sThyh1ik5GnGsThSgbcMS5NjGI0gGpvbYOiUCUD0jttXVpPKICwHGnoMciqgAcec57HKISQAavrVNjENUAjn5nhh9REeD4U9C8iJJ3Mo1OhFEU5THXu2t8iMoAJ8HtNKL22rrFg6gOUMg7pOyIqtZgJSFvBbEiqgRk9tq6xYaoFJDda+sWC6JaQGHvkNIjKgYU9w4pLaJqQIHvkNIhKgcU+YYlDaJ6QKHvkA4jagA8E8Yxk9fWrSFEhTuZRn4axrGwd0jJiFoARb9DSkLUMUUn4t8h7UfUBDjGa+tWH6IuwFFeW7e6EbUByrhxoLg+Ez7Tk2RqybhTAS4uTtDstd4KM85r61GxbL7An73+0Xqxj6z7aYLg8Hez2ey/f/P1TdBjT+TdOABhQPuXw2RqvNdmugR4bYbLqPvapMiIG3ikSozXZrIEeW0Gy5j72qTJlPva5MmQ+9ok6j3k0vdCWHttjhKK9NpMlP772mRL+31t0iXcazNO4r020/R+qkVNSPqzSdYKAsxrK4l/dMdSLUosl5YH3d2RoANOGK/dm6ZwHWNeW7h1L9X42xDz2lxMNRAAzGsD4F53h0SrujqoRfjk2jStbqXCvLYsWy11d0mwHldox9Z4bZ4XvYy7ktQ0+VvPS7Bq4XlT4NYgLlcICvPavGTq1t7UT7PkOIbJKdOEXsl7IamB8vdxjqDwnTci9MqdK8/BcFd6FaF3QeiBOzfqPrwrPYyw9tqiKENt5AYivAMIJkdQmNdWZRoAEjRR7V+Lxa6sttyZd8o052pRD+pqYzuivy+9N0Lvoh5WY4iW5Gxpc9Xwl0frAh/D2o+qN27HTU62+rEs7FyO0H/crt4oTs3Ja6tzaXLawIFPDzCwDRIGwcOn1Wmr5vVUi2bCxtv1YQH9AMlHapqgaVijgbwoXBzWW3zxdRMmrbQalwCk88+fP6dpOkPNDLWouUWNsGgqKgrKMq4ozls1L2kI27m0NZzxMRoffzmOh6PxVTSXEI16fvY4cPGRojOXdk9Y2mjOF81I0dZ044yKI+Tkvu6faMLaaztucvANXCsaioxOFUd7Mw19tPu/0I5ia7872irSQqP/A+vK0xs+0TIUAAAAAElFTkSuQmCC" size="100px" width="100px"></image></top><br><br> 
      <div class="thank-text"> আপনার মতামত সঠিক ভাবে সংগৃহীত হয়েছে। আপনার মূল্যবান মতামতের জন্য ধন্যবাদ</div> 
      <button id="resetBtn" class="reset-btn">New Form..></button> 
      <button id="closeBtn" class="close-btn">Close Form</button> 
    </div> 
  </div> 
 
 
<Script> 
   // ---- logic using hidden iframe so server saves data first ---- 
  const form = document.getElementById('SurveyForm'); 
  const iframe = document.getElementById('hidden_iframe'); 
  const thankOverlay = document.getElementById('thankOverlay'); 
  const resetBtn = document.getElementById('resetBtn'); 
  const closeBtn = document.getElementById('closeBtn'); 
 
 
  let awaitingResponse = false; 
 
  // mark that we've submitted — when the iframe finishes loading, we'll show the thank-you 
  form.addEventListener('submit', function (e) { 
    awaitingResponse = true; // iframe onload will handle UI 
    // allow the form to submit normally (target=hidden_iframe), do not preventDefault 
  }); 
 
  // iframe load happens on initial page load too; only respond when we actually submitted 
  iframe.addEventListener('load', function () { 
    if (!awaitingResponse) return; 
    // show thank-you overlay (centered) 
    document.querySelector('.form-container').style.display = 'none'; 
    thankOverlay.style.display = 'flex'; 
    thankOverlay.setAttribute('aria-hidden', 'false'); 
    awaitingResponse = false; 
  }); 
 
  // Reset button: hard reload (fresh form). The sheet already has the saved data. 
  resetBtn.addEventListener('click', function () { 
    location.reload(); // full refresh to show a fresh empty form 
  }); 
   
   
  closeBtn.addEventListener('click', function () { 
  thankOverlay.style.display = 'none';          // hide thank-you message 
  document.querySelector('.form-container').style.display = 'none'; // also hide form 
}); 
   
   
   
  /*closeBtn.addEventListener('click', function () { 
  form.close();   
  thankOverlay.style.display = 'none'; 
  document.querySelector('.form-container').style.display = 'block'; 
});*/ 
 
 
</script> 
</body> 
</html>

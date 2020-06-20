# hack-Jaipur
Smart door for hotels Key less concept.
<h1>Securite-Version-1</h1><br>
<p>It contains 3 folders: <br><p>1. ESP8266-Device<br>2. Securite<br>3. Database-files</p></p>
<p><b>ESP8266-Device</b> contains the device code, <b>Securite</b> contains the web application and <b>Database-files</b> contains all the databases we have used in both SQL and CSV format.</p>
<p>In <b>Securite</b> two files are there:<br>
  <p>The <b>index.php</b> works for User Registration, Booking, Verification and Check Out.<br>
  The <b>link.php</b> works as virtual key for User to <b>Close</b> & <b>Open</b> room. First the user will have to set its own key for room. On check out the key will be assigned as NULL. One admin login is also available to open or close any room without using key.<br><br>
The device flashed with <b>code.ino</b> file in ESP8266-Device directory will directly fetch the data from server using the rest api(<b><u>securite/api/status.php</u></b>) and act accordingly.
</p>
  <br>
  
  <h1>Firebase-Web-App</h1><br>
<p>It contains 2 folders: <br><p>1. FirebaseArduino<br>2. WebApp</p></p>
<p><b>FirebaseArduino</b> contains the device code and <b>WebApp</b> contains the web application to directly open or close door.</p>
<p>In <b>WebApp</b> 3 files are there:<br>
<p>The <b>index.html</b> works as link to control the <b>Open</b> or <b>Close</b> updation of data in firebase.<br>
The device flashed with <b>ESP8266WiFi.ino</b> code in FiebaseArduino directory will directly fetch the data from firebase and act accordingly.
</p>
  <br>
  <p><b>Note</b>: Check comment lines for more info.</p>

# Get-Location-and-System-Details-Of-others
Use this code to get the ip address and device info of whoever clicks on a particular link , which redirects to this HTML code.
Create a HTML page using the code below and then host it and send the link of the hosted file to any recipient you want to try this on.

CODE -

<html>
<?php
$file = "log.txt";
$ip = $_SERVER['REMOTE_ADDR'];
$date = date("d-m-y");
$time = date("H:i:s");
$browser = $_SERVER['HTTP_USER_AGENT'];
$data = "IP: ".$ip.", Date: ".$date.", Time:".$time.", Browser: ".$browser;

$f=fopen($file, 'a');
fwrite($f,$data."\r\r\n");
fclose($f);
?>
<img src="img.jpg">
</body>
</html>


Use this code to get the ip address and device info of whoever clicks on a particular link , which redirects to this HTML code.

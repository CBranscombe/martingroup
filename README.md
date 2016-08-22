<?php 

header('Content-type: text/xml');
echo '<?xml version="1.0" encoding="UTF-8"?>';
echo '<Response> Talk Back </Response>

?>

$to = curtis@martingroup.ca;
$subject = "Message from {$_REQUEST['From']} at {$_REQUEST['To']}"; 
$message = "You have received a message from {$_REQUEST['From']}. Body: {$_REQUEST['Body']}"; 
$headers = "From: info@martingroup.ca

mail($to, $subject, $message, $headers); 



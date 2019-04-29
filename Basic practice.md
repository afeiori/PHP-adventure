# PHP-adventure
A newbie's self-study footprint for PHP learning. Referrence material: David Sklar (April 2016) Learning PHP. Sebastopol, CA: O'Reilly Media.

<html>
    <head><title>Afei's PHP practice</title></head>
    <body>
        <form method="POST" action="phptest.php">
        Input test: <input type="text" name="zipcode"/>
        <button type="submit">Click</button>
        </form>
    </body>
</html>

<?php
$zipcode=trim($_POST['zipcode']);
$zip_length=strlen($zipcode);
if($zip_length!=5){
    print "please enter a zip code that is 5 characters long.";
}
?>

# PHP-adventure
A newbie's self-study footprint for PHP learning. Referrence material: David Sklar (April 2016) Learning PHP. Sebastopol, CA: O'Reilly Media.

簡易計價計算機

<html>
    <head><title>Afei's Restauran</title></head>
    <body>
        <form method="POST" action="phptest.php">
            Hamburger: <input type="text" name="hbg"/>
            <br>
            Chocolate Milk Shake: <input type="text" name="choco"/>
            <br>
            Coke: <input type="text" name="coke"/>
            <br>
            <button type="submit">Calculate the price</button>
        </form>
    </body>
</html>
<?php
$hamburger=4.95*$_POST['hbg'];
$chocomilkshake=1.95*$_POST['choco'];
$coke=0.85*$_POST['coke'];
$gross=$hamburger+$chocomilkshake+$coke;
$tax=0.075*$gross;
$tips=0.16*$gross;
$total=$gross+$tax+$tips;
print "Your Order:<br>";
print "Hamburger $4.95 * ".$_POST['hbg']." = $hamburger<br>";
print "Chocolate Milk Shake $1.95 * ".$_POST['choco']." = $chocomilkshake<br>";
print "Coke $0.85 * ".$_POST['coke']." = $coke<br>";
print "Sales tax = $tax<br>";
print "Tips = $tips<br>";
print "Total Pay = $total";

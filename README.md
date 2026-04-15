# SeaMiner
A semanitc web semplification attempt

## Usage

seastats.php - display some data stats regarding a website account<br>
seawriter-123sample.php - Write last atomic update in the *semantic* format<br>
seaminer.php - Read last atomic update in the *seamantic* format<br>

es:<br>

// simple query by date<br>
if (seastats.php?op=checkdateforupd&date=20250707&account=root > 0) then<br>
  seaminer.php?account=root&date=20250707<br>
}<br>

// query by last atomic update<br>
$date = (seastats.php?op=lastupd&account=root)<br>
if (seastats.php?date=$date&account=root > 0) then<br>
  seaminer.php?account=root&date=$date<br>
}<br>

// query by last week<br>
$date = (seastats.php?op=lastweek&account=root)<br>
if (seastats.php?date=$date&account=root > 0) then<br>
  seaminer.php?account=root&date=$date<br>
}<br>

// query by last month<br>
$date = (seastats.php?op=lastmonth&account=root)<br>
if (seastats.php?date=$date&account=root > 0) then<br>
  seaminer.php?account=root&date=$date<br>
}<br>

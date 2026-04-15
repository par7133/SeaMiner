# SeaMiner
A semantic web simplification attempt.

## Usage

seastats.php - displays some data stats regarding a website account.<br>
seawriter-123sample.php - An example to write last atomic updates in the *semantic* format.<br>
seaminer.php - Read last atomic update in the *semantic* format.<br>

eg:<br>

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

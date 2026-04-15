# SeaMiner
A semanitc web semplification attempt

## Usage

seastats.php - display some data stats regarding a website account
seawriter-123sample.php - Write last atomic update in the *semantic* format
seaminer.php - Read last atomic update in the *seamantic* format

es:

// simple query by date
if (seastats.php?op=checkdateforupd&date=20250707&account=root > 0) then
   seaminer.php?account=root&date=20250707
}

// query by last atomic update
$date = (seastats.php?op=lastupd&account=root)
if (seastats.php?date=$date&account=root > 0) then
   seaminer.php?account=root&date=$date
}

// query by last week
$date = (seastats.php?op=lastweek&account=root)
if (seastats.php?date=$date&account=root > 0) then
   seaminer.php?account=root&date=$date
}

// query by last month
$date = (seastats.php?op=lastmonth&account=root)
if (seastats.php?date=$date&account=root > 0) then
   seaminer.php?account=root&date=$date
}

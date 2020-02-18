# Extract Apple health data Use Case
1) Open Health on iPhone
2) click on profile (picture of Penny and me)
3) click on export all health data (takes a minute to prepare xml)
3) choose delivery method (Gmail)
4) specify my account and title
5) open Gmail on computer
6) download zip file
7) open zip file from download tray in browser
8) copy to home\Projects\qs_ledger\apple_health\data
9) open command prompt
10) cd Projects/qs_ledger/apple_health
11) python3 apple-health-data-parser.py data/export.xml
12) in command prompt run ==> sudo nautilus
13) In "Other Locations" click on Computer
14) go to var/lib/mysql/lose_weight
15) drag ActivitySummary.csv from data directory into lose_weight folder
16) start MySQL studio
17) open Projects/loseWeight/Load_Day_Activity
18) run script 


# Apple Health Extractor and Data Analysis

The repo was cloned a level up from the apple health branch
Put export.xml in data folder
Ran the parser
	python3 apple-health-data-parser.py data/export.xml
and volia, bunches of .csv files
edited README.md
git pull origin master
git push --set-upstream origin master
git commit -a -m "ready for pushing readme"
git push --all
saved again to update readme
git commit -a -m "ready for pushing readme third time"
git push --all

So, the above shows initial push, then subsequent pushes.
I'm doing another push to get this text up, then done for now.

# Getting Gateway up 
git config --global user.email "Joel@joelbell.net"
git config --global user.name "joelbell"
git remote add origin https://github.com/joelbell/qs_ledger.git
git pull origin mastercd
cd apple_health
Put export.xml in data folder
Ran the parser
	python3 apple-health-data-parser.py data/export.xml

# .csv files
ActivitySummary.csv	Kcals by day
Workout.csv		Kcals, time and distance by workout (lots of workouts not showing)

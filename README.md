<h1>NIST CFReDS Data Leakage, 2015</h1>


<h2>Description</h2>
This project presents the findings from a complete digital forensics investigation conducted on the NIST CFReDS 2015 Data Leakage Case, a publicly available forensic challenge produced by the National Institute of Standards and Technology (NIST).
<br />


<h2>Tools Used</h2>

- <b>Autopsy</b> 
- <b>FTK Imager </b>
- <b>Registry Explorer</b> 
- <b>DB Browser for SQLite </b>

<h2>Screenshots:</h2>

<p align="center">
Registry Explorer: SOFTWARE hive showing OS version, install date, and registered owner 'informant' <br/>
<img src="https://imgur.com/HPiEvXz.png" height="80%" width="80%"/>
<br />
<br />
Registry Explorer: SAM hive showing all user accounts including 'informant'  <br/>
<img src="https://imgur.com/eY71cHg.png" height="80%" width="80%">
<br />
<br />
DB Browser for SQLite: Chrome History query showing browsing activity including data leakage searches on March 23, 2015 <br/>
<img src="https://imgur.com/O6jiW8v.png" height="80%" width="80%">
<br />
<br />
Registry Explorer: NTUSER.DAT RecentDocs showing secret_project files and resignation letter accessed by the suspect:  <br/>
<img src="https://imgur.com/RAqWqmM.png" height="80%" width="80%">
 <br />
<br />
 FTK Imager: Google Drive user_default folder showing snapshot.db and sync_config.db wiped (null byte contents confirmed in hex panel)  <br/>
<img src="https://imgur.com/Y4LmOt8.png" height="80%" width="80%">
<br />
<br />
FTK Imager: FTK Imager: RM#1 exFAT partition showing Secret Project Data folder with hex panel confirming 'Authorized USB' volume label string  <br/>
<img src="https://imgur.com/S2Bo1kz.png" height="80%" width="80%">
<br />
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@

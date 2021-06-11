# timeshift for linux like Windows restore point

In Windows 10, it is called 復元.

# how to install
<pre>
sudo add-apt-repository -y ppa:teejee2008/timeshift
sudo apt-get update
sudo apt-get install timeshift
</pre>

# How to create a snapshot
<pre>
sudo timeshift --create --comments "A new backup" --tags D

--tags D stands for Daily Backup
--tags W stands for Weekly Backup
--tags M stands for Monthly Backup
--tags O stands for On-demand Backup
</pre>

# how to restore a snapshot
<pre>
sudo timeshift --restore
</pre>


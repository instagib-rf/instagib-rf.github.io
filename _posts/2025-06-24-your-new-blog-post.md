## This is my first blog post!

## iCloud Drive Sync on Windows will not progress


After restoring from a crash, my iCloud drive stopped synchronizing and was not updating files. My guess is that iCloud does a sort of local or server-side scanning of files which will cause it to stop processing further files if it fails for a reason.

I had a problem with a Microsoft word document, an Apple Pages document, a Numbers file, and a Keynote file. Once I zipped the offending files, iCloud gave up on scanning them and the synchronization worked fine for all other files. Today it happened another time with another large word document.

I could look in file manager to see files had the 'sync pending' wheel instead of a checkmark throughout a few folders. Here is a set of steps I wrote to fix the issue.

1.	Restart iCloud [Open task manager CTRL + SHIFT + ESC]

    Find iCloud, tap arrow >, right click [iCloud Drive] and left click end task.

3.	Open iCloud from the Task bar in bottom right ^ area or

    from the Windows Button -> Apps -> iCloud

4.	Tap [View in File explorer] from the iCloud application under iCloud drive. This step is unnecessary as iCloud will restart the service, but this is faster, and you may need to do these steps multiple times during troubleshooting.

5.	See if iCloud Drive in task manager Step 1 is using any network or disk usage.
   If so wait until it goes to 0 MB/s and 0 Mbps.

7.	Look at File Explorer to see if your files are updated and no longer show sync pending and ignore what iCloud drive shows on the iCloud application.

8.	If your files still show sync pending>>

    Option One is to zip the folder entirely or the files which are stuck on sync pending. Right click the directory, move cursor to [Compress To...] then left click Zip File.

    Option Two: Pick a directory which has many files still pending then cut -> paste it into a different folder on your hard drive like your Documents folder.

8.	Check task manager again to see if iCloud Drive is updating and synchronizing files. Wait until it is done and goes to 0 MB/s and 0 Mbps.

    Post option one: After zipping the folder or files, delete the files in the directory that you zipped or the offending directory if you zipped the entire directory.

    Post option two: Paste the directory from step 6 back into your iCloud directory of choice.

9.	Check task manager again to see if iCloud Drive is updating and synchronizing files. Wait until it is done and goes to 0 MB/s and 0 Mbps.

At this point you need to divide and conquer, pick option one, option two, or a combination of both. If you stop making progress, start back at step 1 because iCloud Drive frequently gets stalled for some reason or another. All your devices should be able to unzip files or folders you have zipped so no data is lost. You may be able to unzip them, and iCloud will update everything fine synchronizing as before or you will find the offending files which iCloud does not like scanning.

I do not suggest deleting the entire iCloud directory as it will waste time if iCloud Drive gets stuck at the exact same point.


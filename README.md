# Kemono.party-Downloader
This is a quick and dirty kemono.party downloader using python.

## How to use:
1. Install python
2. Install bs4 using the command ```pip install bs4``` 
3. Edit kemono-dl.py and change all four of the cookie values for kemonoparty and change the flag ```I_changed_the_cookies``` from a 0 to a 1 
   - You can get the cookie values from using a [chrome](https://chrome.google.com/webstore/detail/get-cookiestxt/bgaddhkoddajcdgocldbbfleckgcbcid?hl=en) or [firefox](https://addons.mozilla.org/en-US/firefox/addon/cookies-txt/) extension
   - You must pass a cookie value or their ddos protection won't let the script access the site 
4. Place users main page link or post link in the Users.txt file with one entry per line
   - links should look like: https://<span></span>kemono.party/SERVICE/user/USERID or https://<span></span>kemono.party/SERVICE/user/USERID/post/POSTID
5. Run ```python kemono-dl.py``` or with a download location ```python kemono-dl.py "C:\Users\User\Downloads"```
   - If no download location is passed then file will be download to the current working directory
   
## Notes:
- Current file format is ```/Serivce_Name/User_name/[Posts date and time] post title```

## To do:
- [ ] Integrate youtube-dl for downloading external video links
- [ ] Extract all external links to a single file
- [ ] Duplicate files and downloads (Seems to be a problem on kemonos end)
- [ ] Images in content section might not display in Content.html
- [ ] Allow file naming structure to be changed in command line
- [X] Allow file location to be set in command line
- [ ] Allow a cookie.txt file to be read in
- [ ] Add Discord service 

## Keep in mind:
- Using this might get you IP banned from kemono party.
  - This has not happened to me but is a possibility 
- If the site changes the script might break.
- Kemono party places some external links as "files" currently they will not be downloaded.
- Kemono party seems to have files in the download section that are broken.
  - ie the file isn't actually a file

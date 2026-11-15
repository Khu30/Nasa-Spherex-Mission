# Nasa-Spherex-Mission
If someone else (a hackathon judge, teammate, or user) wants to open your project in Microsoft Edge, here is how they can do it:

**Method 1: The Easiest Way (Send them the folder / Open directly in Edge)**
They do not need to install anything (no Python, no Node.js required):

Send them the project folder (or ZIP the folder and share it with them).
Inside the folder, have them go to the static subfolder.
Right-click index.html 
→
→ select Open with 
→
→ choose Microsoft Edge. (Or simply drag and drop index.html directly into an open Microsoft Edge tab).

Command Prompt Shortcut to open it in Edge:

cmd
start msedge "C:\Users\NASA HACKTHON\static\index.html"

**Method 2: Opening via Local Network (Wi-Fi) from Another Device**
If you are running the project on your laptop and your friend/judge is connected to the same Wi-Fi network:

Find your laptop's local IP address:
In Command Prompt, type: ipconfig
Look for IPv4 Address (e.g., 192.168.1.15).
Run the server bound to all networks:
cmd
python -m uvicorn api:app --host 0.0.0.0 --port 8000
The other person opens Microsoft Edge on their laptop or phone and types:
http://YOUR_IP_ADDRESS:8000
(e.g., http://192.168.1.15:8000)

**Method 3: Put it Online for Free (Anyone in the World can open in Edge)**
If you want a public link that anyone on any device can open in Edge anytime:

You can deploy the static folder to GitHub Pages, Vercel, or Netlify Drop:

Go to drop.netlify.com
 (or GitHub Pages).
Drag and drop the static folder into the browser.
Netlify will instantly give you a free live public URL (e.g., https://nasa-spherex-explorer.netlify.app).
Anyone can paste that link into Microsoft Edge on any computer to explore the sky!

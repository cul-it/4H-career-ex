# League of Coders
## Description 
This is a collection of Women in Technology used for teaching purposes at Mann Library for 4-H Career Explorations 2016. We taught middle school (grades 6-8) children from 4-H chapters and schools across New York State.  There were 15 students in each session, and we taught 5 sessions on June 29 and 30, 2016.  Each session was an hour and 25 minutes. This was the first time we taught a coding 
## Team
The planning and instruction team consisted of Darcy Branchini, Huda Khan, Sandy Payette, Tahir Poduska, and Holly Mistlebauer.  Alan McCarty was also pivotal in planning and setting up hosting (for each student instance), and configuring student machines.
Our contact at 4-H was Alexa Maille, NYS 4-H STEM Specialist. 
## Setup 
### GitHub
There are two branches - master - and - instructors. The master branch is the student version, or the beginning point for teaching purposes (lots of placeholders).  
### Hosting
Separate AWS instances were setup for each of the 15 students, plus a few extra (just in case).  Domains were also setup to each of these instances.  We used the following pattern: wit-[nnn].library.cornell.edu. Each of these instances had a working directory and source directory.  The working directory, just as it sounds, was for students to code from.  The source directory allowed us to quickly refresh machines between sessions.  A script was written (by Alan) for this purpose.  It looped through each instance, deleted any files in the working directory, and moved files from the source directory into the working directory.  This allowed us to refresh the machines quickly between sessions to ensure the classroom was ready for the next set of students.
### Workstations
We used classroom B30A in Mann Library. Workstations are PCs with Notepad + + for our text editor.  This text editor came with a plugin, titled NppFTP, that allowed us to connect to each student's working directory on their respective AWS instance and domain (using SSH).  Any code changes were saved to their respective AWS instance instead of the classroom PC.  It was setup this way for two reasons: 1.) We didn't need to setup/run a web server on classroom PCs, or run the application from the file system.  2.) We didn't need to worry about the classroom PC rebooting.  If it does reboot, then the machine is wiped clean so the student would lose their work. We also prepped each student's machine by opening the text editor and browser (Firefox) with their unique domain.  Finally, we kept index cards at each student's machine with their respective/unique domain in case the student or an instructor needed to refer back to it.
## Lessons Learned
- A very large majority of these students don't yet have exposure to HTML.
- Having students type slows down what we are able to fit into the time frame. From session to session, we kept adding more commented out lines and prompted them to uncomment them instead of write them with us. 
- The for loop physical activity/game worked well. 
- The references to something they do know (like variables in algebra) worked well.
- Time goes fast. We tried to teach too much in one hour and 25 minutes.  
- If we do this next year, we need to decide whether it makes more sense to teach three days with high school students or modify our lesson and teach middle school students again.  If we teach middle school students, we should probably stick to web basics, such as HTML, CSS and a tiny bit of Javascript for a simple user behavior.
- It was fun!!!


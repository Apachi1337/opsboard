Opsboard is currently a static HTML Website served by pythons built in HTTP server. 
The command to start the app is:
 "cd ~/projects/opsboard" 
 "python3 -m http.server 8000 --bind 127.0.0.1 --directory site".
 To stop the server its "ctrl+c"

You can verify that its running using two commands:
Curl will show you whether a service is responding over HTTP.
(curl http://127.0.0.1:8000)

SS will show you whether a process is listening on a active port and using -p will show which process owns it.
(ss -lnpt 'sport = :8000')
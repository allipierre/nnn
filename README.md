a) In your browser, go to the Administration login page (4550:10)

b) In a Terminal, go into the directory \utilities\debug and connect with SQL*Plus as SYSDBA
c) alter session current_schema=apex_180100;
d) @d1.sql -> This will show all current debug sessions
e) @d0.sql -> will enable system wide LEVEL9 debugging for APEX

f) Switch back into the browser

g) Click the 'Sign in to Administration' button

h) Switch back to SQL*Plus

i) @d0.sql -> will disable system wide LEVEL9 debugging

j) @d1.sql -> should show a new debug entry for wwv_flow.accept
k) @d2 <debug identifier> -> to get the debug details for both entries

l) upload the debug entries so that we can have a look

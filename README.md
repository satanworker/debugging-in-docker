
This repos helps checking if there are any difference when
debugging remote typescript vs local typescript code.

Use in the following way for checking if local debugging works:
- npm install
- open vscode and set a couple of breakpoints in tssrc/index.ts (in the nested if statement)
- "npm localdebug" from terminal
- run debugger w config "Attach locally" 
- check if "red dot" which indicates a breakpoint changes position after attaching the process and stepping through it

Use in the following way for checking if remote debugging works:
- install Docker for Windows or Docker for Mac
- npm install
- open vscode and set a couple of breakpoints in tssrc/index.ts (in the nested if statement)
- "npm localdebug" from terminal
- run debugger w config "Attach to docker (mac)" or  "Attach to docker (win)"
- check if "red dot" which indicates a breakpoint changes position after attaching the process and stepping through it
NOTE: on windows, be sure to enable the docker option which allows to "export" local fs dir
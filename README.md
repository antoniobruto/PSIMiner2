__________________________________________________________________________

**************************************************************************
                                 PSIMiner

                    ReadME - PSIMiner - IIT Kharagpur
              Created by Antonio Anastasio Bruto da Costa
                  E-mail: antonio.cse.iitkgp@gmail.com

             Principal Investigator: Prof. Pallab Dasgupta

**************************************************************************

	  Use: For Learning Causal Sequences from Time-Series

**************************************************************************

TO BUILD: Run the build-script 'build' in the folder forFET

Requires 
1. C, C++ compilers
2. flex, bison
3. python >2.7

Supported on Linux (Ubuntu >16.xx verified) and MacOSX (Mojave, Catalina verified)

**************************************************************************

TOOL USAGE:
The binary of the tool is built in the "build" directory created by 
build.sh 
If this directory does not exist, please create it before running the build script.

For TraceFiles:
It is assumed that there is a time reference in column 1.
Note that the change of truth for a predicate occurs at the first timestamp
at which the change is observed in the trace data. Hence a change of 
truth for a predicate observed on the last line of the trace file may 
cause unintentended results. 

The prefix of the name of the assertion file will be the name of the config file.

**************************************************************************

A primary (small) example to get you started off can be found in the directory "example".
OTHER EXAMPLES: A broader set of examples are available at:
	https://github.com/antoniobruto/PSIMiner-Examples

**************************************************************************
Updates/Releases

v1.1
- Supports mining differences between targets over sets of time-series.

v1.0
- Mining temporal causal relations from sets of time-series.

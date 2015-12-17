#Installation procedures for bt-http-server
Required Libs: BlueZ (lbluetooth)
# Introduction #

This page contains information on how to compile and run bt-http-server.
Please note that you need lbluetooth library.

# Procedure #
To run the system do the following steps:
  * **1.Compile and Run:**
> > Choose one of the alternatives for this step and proceed to next.
    1. Run the Make file and follow the instructions.
    1. Compile both modules against bluetooth and pthread libraries with one output file.
> > > @ gcc http.c server.c -o sim -lbluetooth -lpthread
    * **2.open (any) web browser and enter the following address in the address bar:**
> > > @ http://localhost:8080/command_center.htm
    * **3.follow the instruction given on the web page to send a message.**
      * for start message, type: START then x cordinates in 5 digits and y cordinates in 5 digits, there's a space character between them.
> > > > @ START 00500 11611
      * for stop message, Type:
> > > > @ STOP
    * **4.to view log file do one the followings:**
      * go to the local path and open .txt file: /web\_pages/log.txt
      * click on the link on the web page.

**note:** after a message is sent, click back to return to home page.
**note:** if the web page returns and error page saying "Failed to Connect" or "Page Load Error", restart the web server.
# PerformanceTest
Technologies used


     Install the latest 64-bit JRE or JDK: https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html
     Download Jmeter: http://jmeter.apache.org/download_jmeter.cgi
 
 
 Development Steps 
 
 
    With Jmeter
         Using Proxy Server: 
       
     1.Open Apache Jmeter
     2.Open Templates->Select Recording on the menu bar
     3.In the HTTP Request Defaults element:
                  Server name or IP and Path
     4.Add Recording Controller for for the scenario
     5.Configuration browser: 
                  Configure your browser to use the JMeter Proxy (same port that is in HTTP(S) Test Script Recorder)
                  Add Certificat apache jmeter (which is in bin).
     6.add listener (for the type of response)
     7.Save Test
     8.Record navigation with start in HTTP(S) Test Script Recorder
     9.Extract Report with commande: jmeter -n -t <jmx_file.jmx> -l <jtl_file.csv> -e -o <html_folder>
     
        Using  BadBoy:
  
     1.Record Script in Badboy ToolE
     2.Export Script To JMX format
     3.Open with Jmeter
     4.Generate HTML Report with :
          cmd line : jmeter -n -t <jmx file.jmx> -l <jtl file.csv> -e -o <html_folder>
                  
 

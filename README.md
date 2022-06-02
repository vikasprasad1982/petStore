# petStore
For 86400 Test Assessment

## Pre-Requiste

- Jmeter 5.4.3
- JDK 1.8

## How to Run the Test

- Start the Jmeter in GUI Mode

> To start the jmeter in the GUI mode

      - In Windows
          - Direct open from Folder
                - <Location of apcahe folder> -> bin ->jmeter.bat (double click)
                - Press Play button
          - From Command Prompt
                - cd <Location of apache folder>/bin/jmeter.bat
                - Press Play button
  
      - In Mac
                - Open Terminal
                - cd <Location of apcahe folder>/bin
                - enter "sh jmeter.sh"
                - Press Play button
               
> To start the jmeter in Non-GUI mode
  
   - Run Command
   /<Location of apcahe folder>/bin/jmeter.sh -n -t /<script_location>/PetStore_CreatePet_API.jmx –l results.jtl –e –o ./results -Javg_resp_threshold=300 -Jnumber_of_iterations=20 -Jerror_count_threshold=1
  
  | Element | Description |
| ------ | ------ |
| < Location of apcahe folder >/bin/jmeter.sh | Path of the jmeter shell script |
| -n | Use Non GUI Mode] |
| -t /<script_location>/PetStore_CreatePet_API.jmx | Path of the jmeter project script |
| -e | Generate report dashboards when test completed |
| –o ./results | Path for the output directory for the report dashboard. |
| -Javg_resp_threshold=300 -Jnumber_of_iterations=20 -Jerror_count_threshold=1 | Sets the test properties (See JMeter Project Structure; Test Plan section for the details of the defined properties). OPTIONAL - As if not mentioned they will set the default values |

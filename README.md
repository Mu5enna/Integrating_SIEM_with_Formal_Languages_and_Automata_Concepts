# Integrating_SIEM_with_Formal_Languages_and_Automata_Concepts


  - The XML file contains a grammar that includes states, an alphabet, a starting state, and production rules. To adapt the program to a different grammar, you 
  only need to edit the XML file as desired and select the updated file from the 'Load XML' section. Additionally, you can specify the number of times each 
  device can violate critical conditions before getting banned.

  - The app reads the XML file and processes the data from the XLSX file according to the rules defined in the XML.

  - Each process step is displayed in the terminal of the app, and it reports whenever a device sends a critical EventID (if the EventID in the log is in the 
  critical list in the XML file). The app saves all records to a file named 'report.txt'.

  - If a device violates critical conditions more than the allowed times specified in the XML file within a day, it gets banned and added to the banned list. 
  This list is stored in a file. Each time the app runs, it reads the previously banned devices from the file and ignores requests from those devices. Users can 
  reset the banned list if needed.

# Note
  - The XML file has rules defined by a DTD located in the "Example Logs & XML" folder. The app will not work if your XML file does not conform to these rules.

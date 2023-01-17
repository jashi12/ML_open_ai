# File Classifier

This repository contains code for classifying files as suspicious or not using the OpenAI GPT model.

OpenAI API credentials can be gotten from [here](https://beta.openai.com/signup/). This is a proof of concept for a scalable solution to investigating MFT logs of compromised endpoints/servers. 

### Data

The code uses a dataframe of file paths, you can use your own dataset or create a new one. This concept is extremely versatile.

### Results

The files that were tested are as follows:

    "/ProgramData/DLLRegisterServer.exe" -> Cobaltstrike beacon
    "/Windows/System32/cmd.exe",
    "/Users/jashi/AppData/Local/Temp/Advanced Port Scanner 2/advanced_port_scanner.exe" -> Reconnaissance tool
    "/ProgramFiles/MicrosoftOffice/Office/EXCEL.exe",
    "/ProgramFiles/Adobe/AcrobatReaderDC/Reader/AcroRd32.exe",
    "/Users/jashi/Documents/executables.zip" -> Generally suspicious .zip file
 
Our model was able to succesfully label all 6 file paths. Additionally testing with larger datasets to come in the future.

## Built With

* [Python](https://www.python.org/) - The programming language used
* [pandas](https://pandas.pydata.org/) - Data manipulation library
* [openai](https://beta.openai.com/) - API to access GPT model

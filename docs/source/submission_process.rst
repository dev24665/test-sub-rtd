Submission process
========

Note: Before you begin the submission, we strongly recommend you use the PDC submission template to collect the information required for a successful submission.

Now you are ready to begin the submission process. You need to follow the steps in the order given in the Submission Overview (image) at the top of this document to avoid duplicating steps

The submission process involves the following major activities,

Creating an instrument to upload raw data
Create a project under which to group the raw data into a Study that was generated using a specific experimental protocol
Upload biospecimen and clinical metadata for the samples used in the Studies
Upload any additional supplementary files
Create an instrument:
----------------  

An instrument is a representation of the mass spectrometer from your lab. Go to create, click instrument, and enter the relevant information about the mass spectrometer used to collect the data. If you are a program member, you will receive an email once approved by the PDC admin or the program lead (PI).

Note: You must be added as an assigned instrument operator to upload data to an instrument unless you are the creator of that instrument.

Upload raw files:
---------------  

Click upload, and in the dialog requesting information, select the instrument you previously created. You can upload directly from your local computer or from the cloud (AWS S3 is supported) if your files are on S3 already.

PDC accepts various proprietary data formats developed by different manufacturers of mass spectrometers such as “.raw”, “.d”; “.wiff”; “.wiff.scan”; “.wiff.mtd”; “.dat”; “.mis”. If you encounter a data format that is not currently supported while uploading to the submission portal, please reach out to the PDC helpdesk for assistance.

Note:

For AB Sciex (formerly Applied Biosystems) series of mass spectrometers, such as the AB Sciex TripleTOF and QTRAP, which produce WIFF format data, it's important to note that multiple files may represent one raw file. In such cases, users are required to upload all associated files together in the same upload.

For Bruker instruments like the Bruker Tims Tof series, where a folder represents one raw file, users should compress individual .d folders corresponding to a single raw file into a single zip file. The compressed file should be named in the format "file.d.zip" to correspond to the original file name.

Tip: You may create a separate instrument for each study that you would like to create, even if all those files are generated from the same mass spectrometer. This is not required, but may help to organize and separate your files, facilitating study creation.


Validate file metadata:
--------------  

To use these files to create your studies, you must first validate the file metadata. This ensures that the upload was successful, and no file corruption or truncation has occurred. To do this, you will need the "File_Metadata" sheet from your PDC Data Submission Template saved as a TSV file.

Once you have the TSV file, return to the workspace and look for your program under the "My Programs" section in the left panel. From there, click on the "Instruments" link under your program name.

Locate the name of the instrument you uploaded your files to and select the 3 vertical dots in front of your instrument name.

Click "Validate File Metadata." In the pop-up window, click "browse files" and select the TSV file that you created from the "File_Metadata" worksheet, and click Upload.

A verification log will appear listing which files:

Were successfully validated.
Were not present in your instrument but are present in the TSV file.
Were present in the instrument but missing from your TSV file.
Have failed verification.

If you have files that failed verification, click on the 3 vertical dots in front of your instrument name and select “Show Files”. Within the metadata verification column, click on the “Failed Verification” text to open a window showing the metadata differences.

These differences may be the result of corruption or truncation of the file when uploading to Workspace. Check your metadata worksheet and make sure the values are correct; if they are, then you will need to delete, re-upload and validate the failed files. Once all files have successfully validated, they may be used in the creation of your studies.

Create a Project:
-------------  

Before you can create a Study or add your Protocol, you first need to create a Project.

Click Create->Project to open the wizard. Next, give your Project a name, select a Program and area of Research. You may also add collaborators to your project using the Sharing tab.

Create a Protocol:
--------------
  
Next, you will add the protocol metadata used in your Study. Click Create->Protocol to open the wizard. Required fields are marked with *. If you are unable to complete your protocol, you can ‘Save as Draft’ and resume later.

You can locate your protocol draft using the left navigation panel. Under “View Type” Click “My” and under “Data Type” click “Protocol drafts.” Locate your protocol name and click the vertical dots in front of your protocol name for a menu to appear.

Click "Edit" and proceed with entering your protocol data.

If you feel that the wizard does not adequately meet your annotation needs for your particular Protocol, please contact the PDC by email for help resolving any issues.


Create a Study:
--------------  

In the PDC workspace, a study is a group of instrument raw files that are generated using a specific experimental protocol, with a well-annotated experimental design (sample to file mapping) that can be analyzed through a single bioinformatics pipeline.

To create the study, click Create->Study to launch the wizard. In the wizard, for steps requiring you to enter data in tabular form for the sample/aliquot to file mapping, you may copy and paste from the Experimental Run Metadata sheet from the PDC submission template you prepared. If you are unable to complete your study, you can click ‘Save as Draft’ to resume later.


You can locate your study draft using the left navigation panel. Under “View Type” Click “My” and under “Data Type” click “Study drafts.” Locate your study name and click the vertical dots in front of your study name for a menu to appear.

Click "Edit" and proceed with entering your study data.







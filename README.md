# Audacity_Macros


## OVERVIEW ##
Here you will find .txt files you can import using Audacity's Macro Manager. You can batch apply these macros to a single file or a large number of audio files. 

### Available Macros ###
- "Split_Left": Split a stereo recording to isolate the left-channel and create a mono recording.
- "Split_Right": Split a stereo recording to isolate the right-channel and create a mono recording.
- "Merge_Both": Merge 2 channels of a stereo recording to a single channel.


## USAGE ##
*Audacity makes frequent updates which can change the macro commands, see [CREATE_AND_TEST_MACROS](CREATE_AND_TEST_MACROS.md) to see if the script works properly for your purposes. 

### To Use in Audacity V.3.7.4 ###

1. Download or copy the macro to a text file in a location on your computer where it will live.
2. Open a new blank Audacity project (i.e. open audacity, you should see no tracks open).
3. Select Edit>Preferences, go to Directories. 
4. Beside "Macro output" select Browse and choose the output folder where you'd like to put the resulting audio files. Click Select folder, then OK.
		*Note: If you select the same output folder as your input folder, you will over-write your original files.
5. Select Tools>Macro Manager>import
6. Use the file picker to select the macro text file in the location you downloaded it to.
7. Use "Files" to select a series of files you wish to apply the macro to.

Allow the macro to run, review the files to ensure the macro was applied as preferred. 

You can also apply this macro you've saved to the Macro Manager to a single file by:
1. Selecting Tools>Apply Macro...
2. Select the macro you saved from the list.

## CONTACT ##
Code provided is as-is, with no guarantees. If you have questions or issues you may wish to submit an issue or contact us directly at info@avianeco.com.

## LICENSE ##
These Audacity Macros are licensed under an MIT License to Tyne Baker, and A/Vian Ecological Consulting Inc.

## PLATFORM TESTING ##
These scripts have only been tested on Windows. 

Last platform test peformed on 9JUL2025 with:
- Audacity V. 3.7.4

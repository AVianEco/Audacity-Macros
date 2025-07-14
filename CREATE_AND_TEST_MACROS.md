# Creating and Testing Audacity Macros

## OVERVIEW ##
*Audacity makes frequent updates which can change the macro commands. See [README.md](README.md) to see the last version and date these macros were tested in Audacity.
If you are using a newer version of Audacity than that listed in the [README](README.md), or if you'd like to preview the changes the macro creates to the file before applying broadly see the testing proceedure below.

## TESTING A MACRO FOR STEREO AUDIO MANIPULATION ##
There are several [Macros](MACROS/) in this Repo that manipulate stereo tracks (i.e. `Split_Left`,`Split_Right`,`Merge_Both`). To these you will need to create a new stereo track for testing in Audacity.

### Create a Stereo Tester Track
Follow the steps below to create a test track that will allow you to see the effects of the above listed macros.

#### Generate a new Mono Track:
1. Open a new, empty project.
2. Go to `Generate > Tone...`
3. Use the settings:
   - Waveform = Sine,
   - Frequency=500,
   - Amplitude=0.8,
   - Duration=5s
4. Click `OK`.

#### Add a Second Mono Track
1. Right click on blank space below the existing track. Select `Add Mono Track` from the menu.
2. Click to highlight that new track and select `Generate > Tone`
3. Use the same settings as above but choose another distinct frequency (e.g. Frequency = 5000 Hz) to make this track distinguishable.

#### Merge the 2 Tracks as 2 Channels in a Stereo Test File
1. Click the three dots `...` in the left hand bar of the first track.
2. Select `Make Stereo Track` from the menu.

### View as Spectrogram
The easiest way to see the changes applied by the macro will be to view the file as a spectrogram.
1. Click the three dots `...` in the left hand bar of the first track.
2. Select `Spectrogram`.
3. If desired change the colour and scaling of this spectrogram under `... > Spectrogram Settings`.

### Import the Macro
Follow the instructions in the [README](README.md) to import the desired macro.

### Apply the Macro to the Test file
1. Select `Tools > Apply Macro...`
2. From the list select the new macro you'd like to test.
3. Select a location you'd like to save the output.
4. Open that output file in Audacity to see if the desired effect occured
   - e.g. only the "left" 500Hz tone is still present as a mono file when using the `Split_Left` macro.

## CREATING AND TESTING NEW MACROS ##
You can use the above proceedure to create a test tone that you can use to test any macro you build in the Macro Manager.

### Create your own Macro
1. Create the test file as above.
2. Click `Tools > Macro Manager`.
3. Select `New` to create and name a new macro.
4. Ensure `END` is highlighted in the list of steps then select `Insert`.
5. Add any of the functions (e.g. select track, stereo to mono), adding one at a time.
6. After each new line is added to the steps, select `Save`.
7. Test the steps you've applied to see if they perform as expected.
8. Continue adding steps to build up your macro, testing in between for desired performance.

Once the macro is complete and performing as expected, you can apply it to a single track by selecting `Tools > Apply Macro...` and selecting the new macro from the list. 
Alternately, you can select `Macro Manager > Files` to find and select a list of files. If using the macro manager to apply to multiple files do not forget to go into `Edit > Preferences > Directories` and select your Macro output directory.

### Save and Export your Macro.

If you'd like to save share your Macro, as I have here:

1. Go to  `Tools > Macro Manager`
2. Select the macro you've tested and wish to export from the macro list.
3. Select `Export`, then save the text file to your preferred location.

# How can I add my library to the Library Manager?

The Arduino Library Manager is a feature of the Arduino IDE (Sketch > Include Library > Manage Libraries...) which makes it easy for users to find, install, and update both official and 3rd party libraries. 

When your library is added to the library list every release/tag version of the library in your repository will automatically be made available for installation via Library Manager. 

The users can set their preferences to display an update notification when a new version of any installed library on the list is available and easily update to the new version with just a couple clicks. More information [here](https://www.arduino.cc/en/Guide/Libraries#toc3).

* The library repository must be hosted on a major git-hosting website like GitHub, BitBucket or GitLab (other hosting sites may be considered on request).
* Ensure your library is compliant with [1.5 format](https://github.com/arduino/Arduino/wiki/Arduino-IDE-1.5:-Library-specification) (1.5 format folder layout is not required)
* Your library must not have the same library properties name value as another library previously added to the Library Manager index.
* [Tag](https://git-scm.com/book/en/v2/Git-Basics-Tagging) it and push the tag (or create a release if you web hosting offers a way to do it, for example with [GitHub "releases"](https://help.github.com/articles/creating-releases/)).
* Open an issue on [Arduino's GitHub](https://github.com/arduino/Arduino/issues), specifying the URL of the repository from where to download your library. If you have multiple libraries to submit you are welcome to do them all in a single issue.
* After some days, a member of the Arduino team will add your library to the Library Manager index and close the issue. Shortly after that your library will be available for installation via Library Manager.




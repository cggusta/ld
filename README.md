# LaunchDarkly Technical Homework
I went simple here with a JavaScript SDK implementation, which is segmenting based of a 'firstName' attribute that is pulled from the url query params.

# Setup:
1. Create a flag in your production environment.
    * Set targeting rules to: "firstName" is one of "{choose a first name}"
    * set the rule to serve the Variation 1 experience (true).
    * Set default rule to serve the Variation 2 experience (false).
2. Activate the flag and save.
3. Grab ld-test.html and load it locally in your browser.
    * Edit the user variable to change out the firstName, name and key with whatever you are targeting in the LD UI.
    * Edit the flagDetails variable to change your flag key and the Client-side ID of the project that flag resides in.
4. Add the query parameter "name={insert first name}" to your URL, this is what is the application is looking for.
5. ld-test should now reflect your feature flag.

<img width="800" alt="ld_preview" src="https://user-images.githubusercontent.com/30939099/163898658-aeda3985-ac6f-40b6-ac52-f7686f069611.png">

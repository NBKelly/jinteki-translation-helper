This is available on greasyfork here: https://greasyfork.org/en/scripts/552721-translation-helper

## What does this do
This highlights untranslated elements on a web page, and lets you alt+click on them to open up ftl playground with 
the relevant information so you can play around with it without needing to look through internal code to do so.

<img width="888" height="832" alt="highlight" src="https://github.com/user-attachments/assets/f66da2e9-9688-40bb-97e8-9d967fee0525" />

<img width="1888" height="316" alt="highlight-2" src="https://github.com/user-attachments/assets/93f8cc62-c765-485a-8f6b-aa5a6d327a89" />


## This is cool and I want it to work on my website
You must do the following:
* you'll be using fluent already
* Take all of your elements with their translation key, parameters if appropriate, and if the translation was successful you should include `data-i18n-successful=true` ie `<span data-i18n-key="landing_welcome-welcome" data-i18n-param-username="bob"> (translation) </span>`
* You should probably set up helpers so you never need to manually tag anything
* You'll need to modify the domain of the userscript, and the target location for the ftl file (or files, if you have multiple locations)

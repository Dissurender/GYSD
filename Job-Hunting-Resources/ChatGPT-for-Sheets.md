### Getting started

Setup:
* [Install GPT for sheets](https://workspace.google.com/marketplace/app/gpt_for_sheets_and_docs/677318054654)
* [Create an openAI API key (direct link)](https://platform.openai.com/account/api-keys)
* [Create an openAI API key (guide)](https://gptforwork.com/setup/how-to-create-openai-api-key)
* [Set up your API key in Google Sheets](https://gptforwork.com/setup/how-to-set-up-api-key)

### How do???
* Once you have the Sheets extension set up, paste this function into cell A1: =GPT_TABLE("Give me a list of 5 tech companies in [city name], their CEOs, and their CTOs")
* Limited to 5 for now due to ChatGPT's limitations

* Then paste this function into cell D2 and drag down to generate messages for the rest of the companies you've found so far: =GPT(CONCAT("Please write a 200 word linkedin connection message to",B2))
* Finally, paste this function into cell E2 and drag it down as well: =GPT(CONCAT("give me a coffee chat question for",C2))

---

Or do it all the manual way:
* Copy and paste this search into google, customizing it for either remote roles or roles within a specific city: site:dice.com | site:indeed.com | site:angel.co | site:lever.co | site:greenhouse.io | site:jobs.ashbyhq.com | site:app.dover.io (engineer | developer) ("javascript" AND "remote") -senior -staff -sr. -lead -principal -angular after:2023-02-01
* Highlight + copy the text from the first 5 or so results and [ask ChatGPT](https://chat.openai.com/auth/login) for the names of the companies in those results
* From there you can use ChatGPT to find those companies' CEOs, CTOs, or engineers etc. and message them the same as you would above.

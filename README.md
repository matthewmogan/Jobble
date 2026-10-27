# Jobble

Guess the country from how its people work.

Each day Jobble shows one country's total number of jobs and a treemap of how those jobs split across agriculture, industry and services, for women and men. You get six guesses. Every wrong guess shows the distance and direction to the answer (capital to capital) and unlocks a clue: unemployment, how people work, region, income group, then the capital's first letter.

**Play:** https://matthewmogan.github.io/Jobble/

## How it works

- One static page, `index.html`, with no build step and no dependencies.
- Figures load live in the browser from the [World Bank Indicators API](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392) (free, no key). They are the ILO's modelled estimates from the World Development Indicators.
- Total jobs = labour force × (1 − unemployment rate).
- The daily country is picked from the same shuffled list for every player, so everyone gets the same puzzle each day. Practice mode serves random countries.
- Stats, streaks and today's progress are saved in the browser's local storage.

## Run it locally

Open `index.html` in a browser. Opening it inside an app's preview pane won't work, because previews usually block outside data requests.

Data: World Bank, CC BY 4.0.

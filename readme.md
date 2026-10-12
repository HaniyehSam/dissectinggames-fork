# Dissecting Games

Cards to help you analyze a game from different perspectives.

[`dissectinggames.csongorb.com`](http://dissectinggames.csongorb.com)

## Structure

This repository holds **content only**. Everything that displays the cards comes from [cardsimulator](https://github.com/csongorb/cardsimulator), included as a git submodule (pinned to a commit).

- `cards/cardset.xml`: title, repository and public address (used by the QR codes in PDFs)
- `cards/cardCategories.xml`, `cards/cards.xml`: the cards
- `texts/`: documents linked from the cards
- `index.html`: tiny loader, identical in every card set
- `.github/workflows/deploy.yml`: publishes the site to GitHub Pages on every push to `main`
- `cardsimulator/`: the simulator (submodule)

Run locally with any static web server (the XML can't be loaded from `file://`): `python -m http.server`, then open http://localhost:8000/.

Update the simulator: `git -C cardsimulator pull origin main`, then commit the changed `cardsimulator` pointer.

## Version-History

### Todos

- ?

### Release 1.1.2 (Work in Progress)

- shortened descriptions to make cards more readable 

### Release 1.1.1 (26. March 2021)

- minor re-arrangement of the cards in the rows

### Release 1.1 (17. September 2019)

- added new example cards

### Release 1.0 (20. March 2018)

- added cards
	- added question cards
	- added task cards

## Credits

- **Adrian Ace Köhlmoos**
	- [ace2win.itch.io](https://ace2win.itch.io)
- **Csongor Baranyai**  
	- csongorb (at) gmail (dot) com  
	- [www.csongorb.com](http://www.csongorb.com)
- additional input by
	- **Sebastian Stamm**
		- [www.the-stamm.com/](http://www.the-stamm.com/)
	- **Florian Berger**
		- [florian-berger.de/](http://florian-berger.de/)

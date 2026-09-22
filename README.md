# Victory Orobosa's Portfolio

This is the code for my personal portfolio site. You can see it live at
https://victoryorobosa.netlify.app.

I'm a Computer Science student at the University of Central Arkansas, graduating in
Spring 2027. The site covers three projects I've built:

- [AI Supply Chain Intelligence Platform](https://github.com/victory113/supply-chain-analyzer):
  upload a shipment spreadsheet and get KPIs, a risk score, and explanations of what's
  driving it. There's also a [live demo](https://supply-chain-analyzer.netlify.app/).
- [SearchFlix](https://github.com/victory113/searchflix): a movie search engine over
  12.4 million IMDb titles that I used to benchmark seven data structures against each other.
- [Double DQN Lunar Lander](https://github.com/victory113/dqn-lunar-lander): a
  reinforcement learning agent, plus an experiment comparing two versions of the algorithm.

My resume is on the site too:
[Victory-Orobosa-Resume.pdf](https://victoryorobosa.netlify.app/assets/Victory-Orobosa-Resume.pdf).
You can also find me on [LinkedIn](https://www.linkedin.com/in/victory-orobosa/).

## How it's built

It's one page written in plain HTML, CSS and JavaScript, so there's nothing to install
or build. Everything lives in `index.html`, and the images and resume are in `assets/`.

To run it locally, open `index.html` in a browser. I use the Live Server extension in
VS Code, which serves it the same way Netlify does.

The site is hosted on Netlify and redeploys automatically whenever I push to `main`.

## Adding a project

Each project on the page is an `<article class="project">` block in `index.html`. To add
one, I copy an existing block and change the text, links and screenshot.

---
layout: page
title: Projects
permalink: /projects/
---

The following details several projects pursued in the last year or so. It's not a complete list, but aims to evidence some technical skills.

---

## [Dito](https://github.com/winstonjay/Dito)

Dito is a toy interpreted procedural programming language written in Go to learn about parsers, interpreters etc. It uses a basic tree walking interpreter executing straight from the abstract syntax tree which is created via top-down operator precedence parsing. It has become a personal playground for experimenting with different syntax and design patterns, generally avoiding the object oriented paradigm. Here is a code sample finding the total number of ways a target number can be made given a set of coins.

```python
def coinSums(coins, target) {
    let sack = array(target+1)
    sack[0] = 1
    for coin in coins {
        for i in range(coin, target+1) {
            sack[i] += sack[i-coin]
        }
    }
    return sack[target]
}

let coins  = [1, 2, 5, 10, 20, 50, 100, 200]
let target = 200

print(coinSums(coins, target))
```

---


## [Digital Citizens](https://winstonjay.github.io/digitalcitizens/)
New Media MA independent research blog concerning citizen media and democracy in the digital age. Makes use of a variety of natural language processing techniques such as word vector representations, topic modelling and keyword extraction algorithms. This is done to make inferences from textual data to inform studies of cultural phenomena comparatively across online platforms.

---

## [WikiGraph](https://github.com/winstonjay/scrapbook/tree/master/wikigraph)
Finds paths between wikipedia articles and other related functions using the [wikimedia API](https://www.mediawiki.org/wiki/API:Main_page). A path is created by linking articles by the links they contain, just like the [wikipedia game](https://en.wikipedia.org/wiki/Wikipedia:Wiki_Game). See blog post [https://winstonjay.github.io/posts/homunculus](https://winstonjay.github.io/posts/homunculus) for more info on project motivations.

---

## [Hangmanteau](https://github.com/winstonjay/hangmanteau)
Like the traditional game of hangman, only using made up portmanteau words. Developed and deployed on Facebook messenger and web interfaces. Due to changing directions in the project and maintenance needed to keep up with API changes, the project isn’t currently online, code branch for the [previous php implementation is on GitHub](https://github.com/winstonjay/hangmanteau/tree/prev). A key question the project currently faces is what constitutes a good made up word?

<a href="https://github.com/winstonjay/hangmanteau" target="blank">
<img src="../assets/imgs/projects/hangmanteau.png">
</a>

---

## [Movie Review Generator](https://github.com/winstonjay/scrapbook/tree/master/movie_reviews)
Creates movie reviews for a given film by scraping rotten tomatoes and using Markov chains to generate some new ones.

Editors top picks:

* *'I watched this wonderful movie for the integrity of it.'*
* *'If you negatively reviewed this movie, and none of them were resolved by the end of the movie, you are crazy.'*

---

## [Unbeatable Tic Tac Toe](https://instaserfs.eu/tictactoe/)

Implementation of the classic tic tac toe game against an AI opponent using min-max search with alpha-beta pruning to decide which moves to make. Whilst your playing the opponent tells you your opponents 'reasoning'. 🍑 Website has a nice animated UI (no internet explorers though).

<a href="https://instaserfs.eu/tictactoe/" target="blank">
<img src="../assets/imgs/projects/tictactoe.png">
</a>


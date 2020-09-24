---
layout: post
title: Video Game Sales
subtitle: Ranked by Publisher
cover-img: 
thumbnail-img: /assets/img/vg-sales-avg.png
share-img: /assets/img/path.jpg
tags: [python, datascience, buildweek]
---
## My Question
I want to know which publisher is best. (Basic Answer: Nintendo. But keep reading if you want to see how I came to that!)

## My Reasoning
I have always had a strong interest in and love for video games! I'm a particularly a big fan of Nintendo (honestly, a part of me was doing this to prove to myself and others that Nintendo is the best). But which publishers are worth sticking with over time. Which ones provide the most material? I've always thought it was Nintendo, personally, but now I know! And I also know a lot more about other publishers as well!

## My Clarification
The word *best* can be very ambiguous. So, I decided that I would use this data to measure the publishers against each other in two ways:
- The number of unique games each company has made.
- How many copies the average game from each company  sells.

I should also clarify that the games here are only included in the data if they both a) sold a minimum of 100,000 copies, and b) were made before 2017 (I'm not sure quite how early).

### Graph #1: Unique Games
For this graph, I graphed the number of game entries per publisher against their respective publishers.

![graph of unique games made by each publisher](/assets/img/vg-sales.png)

I made this graph first and was happy to see that Nintendo was at least in second place for sheer number of games they had actually made. But when I saw that Namco was in first place, it made me realize I had only been testing for quantity, but not necessarilly quality. It's hard to graph quality, because it's just such an artistic attribute.
### Graph #2: Average Number of Copies Sold per Game per Publisher
I came to the realization that one way to measure quality is by the number of people that buy a product. If everyone is buying it, that usually means it's a pretty good game! So, I took the the number of copies sold for every game for every publisher. I averaged those numbers to make this next graph!

![graph of average number of copies sold per game for each publisher](/assets/img/vg-sales-avg.png)

Not only was I very happy to see that Nintendo found it's way to the top, but that Nintendo was first by a LONG SHOT!! Microsoft came in second on this graph but barely has more than half the average that Nintendo has. In other words, on average, any given game made by Nintendo sells 2.58 MILLION copies! Another very interesting fact is that between this graph and the last, Microsoft and Sony basically switch places. Suggesting that, while PlayStation gets way more games, Xbox sells way more of their exclusive games. Now, one reason this may be is because, for most everyone that isn't super into these two consoles, you think of Xbox, you think of Halo. PlayStation, on the other hand, has many classic exclusives, but it seems that not everyone got way on board with every game.

So, I'm happy to report that Nintendo really is the best! I'm also happy to have learned more about the relationships of Microsoft's and Sony's games with their consumers!

---

sources:
* [Kaggle Vigeo Game Sales Dataset](https://www.kaggle.com/gregorut/videogamesales)
* [My personal Google Colab where I did all the coding (Github copy)](https://github.com/jrivest2/build_week1/blob/master/Justin_Rivest_Buildweek1_Video_Game_Sales.ipynb)
